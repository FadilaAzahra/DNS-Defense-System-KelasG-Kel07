# DNS-Defense-System-KelasG-Kel07
DNS Defense System – Cyber Security | Kelompok 7 Kelas G
  DNS Defense System
  
## Nama Anggota:
1. Mikhail Hibrizi/J0404231087/Network Engineer
2. Fadila Azahra/J0404231087/Lead Analyst
3. M. Qyblat Ilmy Mahdi/J0404231051/Security Analyst

## Deskripsi

Proyek ini mensimulasikan serangan DNS Spoofing dan DNS Tunneling pada lingkungan virtual untuk memahami proses serangan, deteksi, dan mitigasi dari perspektif SOC Analyst.

## Tujuan

1. Membangun infrastruktur DNS lokal.
2. Melakukan simulasi DNS Spoofing menggunakan Ettercap.
3. Melakukan DNS Tunneling menggunakan Iodine.
4. Memonitor aktivitas jaringan menggunakan Security Onion dan tcpdump.
5. Melakukan analisis insiden dan mitigasi.

## Komponen

* Ubuntu Server (192.168.56.10)
* DNS Server BIND9 (192.168.56.20)
* CyberOps Client (192.168.56.30)
* Security Onion (192.168.56.40)
* Fake Server (192.168.56.99)

## Hasil

* DNS Spoofing berhasil mengalihkan client ke fake website.
* DNS Tunneling berhasil membangun kanal komunikasi melalui DNS.
* Aktivitas serangan berhasil diamati menggunakan tcpdump pada Security Onion.
