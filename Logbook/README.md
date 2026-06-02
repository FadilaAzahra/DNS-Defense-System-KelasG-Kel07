
🔹 Minggu 1–3: Fase Setup & Inisialisasi

Target:
Instalasi Virtual Machine (VM) dan konfigurasi jaringan dasar.

Aktivitas:

• Instalasi Ubuntu Server untuk DNS Server dan Attacker
• Konfigurasi Internal Network dengan nama "dmz" pada VirtualBox/VMware untuk isolasi trafik
• Perancangan topologi Star menggunakan Switch-dmz di Cisco Packet Tracer
• Konfigurasi alamat IP pada seluruh host
• Pengujian konektivitas antar host menggunakan ICMP (ping)

Status:
✅ Selesai – Seluruh VM berhasil saling terhubung dan komunikasi jaringan berjalan normal.

────────────────────────

🔹 Minggu 4–7: Fase Hardening & Baseline

Target:
Penguatan keamanan sistem dan pembuatan baseline normal.

Aktivitas:

• Konfigurasi Bind9 pada DNS Server untuk domain [www.lab.local](http://www.lab.local)
• Implementasi Firewall (UFW)

* Default: deny incoming
* Allow: Port 53 TCP/UDP
  • Implementasi logging menggunakan Security Onion
  • Monitoring trafik ICMP dan DNS Query
  • Visualisasi log pada Kibana
  • Pengujian resolusi DNS dari Client

Artefak:

• Screenshot Kibana Log
• Screenshot Konfigurasi Bind9
• Screenshot Status UFW
• Hasil Pengujian DNS

Status:
✅ Fase Hardening dan Baseline berhasil diselesaikan.

────────────────────────

🔹 Minggu 8: Evaluasi & Review Progres

Target:
Validasi kesiapan sistem sebelum fase serangan.

Aktivitas:

• Review infrastruktur bersama asisten laboratorium
• Validasi konfigurasi DNS Server
• Validasi Security Onion dan Kibana
• Verifikasi seluruh log berhasil direkam
• Finalisasi dokumentasi baseline

Status:
✅ Sistem dinyatakan siap memasuki fase ofensif.

────────────────────────

🔹 Minggu 9–10: Fase Serangan DNS Spoofing

Target:
Melakukan simulasi DNS Spoofing (Pharming).

Aktivitas:

• Persiapan VM Attacker
• Vulnerability Scanning menggunakan Nmap
• Konfigurasi website phishing pada Attacker
• Manipulasi DNS Record
• Simulasi pengalihan domain menuju website phishing
• Pengujian akses domain dari Client

Artefak:

• Hasil Scanning Nmap
• Screenshot Website Phishing
• Bukti Redirect Domain
• Screenshot Hasil DNS Spoofing

Status:
✅ DNS Spoofing berhasil dilakukan dan Client berhasil diarahkan ke website phishing.

────────────────────────

🔹 Minggu 11: Monitoring dan Deteksi Serangan

Target:
Mendeteksi aktivitas serangan menggunakan Security Onion.

Aktivitas:

• Monitoring trafik DNS pada Security Onion
• Analisis event melalui Kibana
• Identifikasi Source IP dan Destination IP
• Analisis aktivitas DNS Query
• Korelasi log antara Client, DNS Server, dan Attacker

Artefak:

• Screenshot Security Onion
• Screenshot Kibana Dashboard
• Log DNS Query
• Bukti aktivitas jaringan

Status:
✅ Aktivitas serangan berhasil terdeteksi dan direkam oleh sistem monitoring.

────────────────────────

🔹 Minggu 12: Analisis Insiden

Target:
Melakukan investigasi terhadap serangan DNS Spoofing.

Aktivitas:

• Analisis kronologi serangan
• Identifikasi root cause
• Analisis pola komunikasi jaringan
• Verifikasi proses pengalihan domain
• Dokumentasi hasil investigasi

Artefak:

• Laporan Analisis Log
• Diagram Kronologi Serangan
• Dokumentasi Root Cause Analysis

Status:
✅ Penyebab serangan berhasil diidentifikasi sebagai manipulasi resolusi DNS yang mengarahkan Client ke website phishing.

────────────────────────

🔹 Minggu 13: Mitigasi dan Hardening Tambahan

Target:
Mengurangi risiko terjadinya DNS Spoofing.

Aktivitas:

• Review konfigurasi DNS Server
• Penambahan aturan keamanan firewall
• Pembatasan akses konfigurasi DNS
• Implementasi hardening tambahan pada DNS Server
• Pengujian ulang setelah mitigasi

Artefak:

• Screenshot Konfigurasi Mitigasi
• Screenshot Firewall Rule
• Hasil Pengujian Pasca Mitigasi

Status:
✅ Mitigasi berhasil diterapkan dan risiko manipulasi DNS berhasil dikurangi.

────────────────────────

🔹 Minggu 14: Dokumentasi dan Presentasi Akhir

Target:
Menyusun hasil proyek dan melakukan presentasi akhir.

Aktivitas:

• Penyusunan laporan akhir
• Penyusunan slide presentasi
• Dokumentasi seluruh artefak proyek
• Persiapan live demo
• Evaluasi hasil implementasi

Artefak:

• Laporan Akhir
• Slide Presentasi
• Log Monitoring
• Dokumentasi Mitigasi

Status:
✅ Proyek selesai dan siap dipresentasikan.

────────────────────────

🏁 Hasil Akhir Proyek

• Infrastruktur DNS Server berhasil dibangun menggunakan Bind9.
• Security Onion berhasil digunakan sebagai sistem monitoring dan analisis log.
• Simulasi DNS Spoofing berhasil mengalihkan Client ke website phishing.
• Aktivitas serangan berhasil dideteksi melalui Security Onion dan Kibana.
• Analisis insiden berhasil mengidentifikasi akar penyebab serangan.
• Mitigasi dan hardening tambahan berhasil diterapkan untuk meningkatkan keamanan sistem.
