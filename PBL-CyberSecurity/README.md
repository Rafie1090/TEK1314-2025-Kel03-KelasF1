# Logbook Proyek PBL Keamanan Siber - Kelompok 3

**Skenario:** Network Perimeter Guard – Simulasi Denial of Service (DoS) pada Router Gateway / Firewall

**Anggota:**

1. Senthelee Vannessa Lai – Project Manager
2. Hafiz Tiftazani – Security Engineer
3. Alicia Maharani – Network Analyst
4. Rafie Hafizhsatryo – Lead Analyst

---

# Log Aktivitas Mingguan

## Minggu 1–3 : Fase Setup

**Target**
- Menentukan skenario proyek.
- Membangun lingkungan virtual untuk simulasi.

**Update**
- Install VirtualBox.
- Install Kali Linux sebagai attacker.
- Install MikroTik CHR sebagai Router Gateway.
- Install Ubuntu Desktop sebagai Client dan Analyst.
- Menyusun topologi jaringan.

**Kendala**
- Penyesuaian konfigurasi jaringan antar Virtual Machine agar seluruh perangkat dapat saling berkomunikasi.

**Solusi**
- Mengatur mode adapter dan konfigurasi IP pada setiap VM.

**Artefak**
- Screenshot topologi jaringan.
- Screenshot VirtualBox.

---

## Minggu 4–7 : Hardening & Baseline

**Target**
- Memastikan jaringan berjalan normal sebelum pengujian.

**Update**
- Konfigurasi IP Address seluruh perangkat.
- Pengujian konektivitas menggunakan perintah ping.
- Capture trafik normal menggunakan Wireshark.

**Status**
✅ Fase baseline selesai.

**Artefak**
- Screenshot hasil ping.
- Screenshot capture Wireshark.

---

## Minggu 8–11 : Fase Serangan (Offensive)

**Target**
- Melakukan simulasi serangan Denial of Service.

**Update**
- Melakukan ICMP Flood menggunakan hping3.
- Melakukan TCP SYN Flood.
- Melakukan UDP Flood.
- Monitoring trafik menggunakan Wireshark.
- Monitoring resource MikroTik.

**Hasil**
- Terjadi lonjakan trafik menuju Router Gateway.
- CPU Router meningkat saat serangan berlangsung.
- Client mengalami gangguan akses jaringan.

**Artefak**
- Screenshot terminal hping3.
- Screenshot Wireshark.
- Screenshot Resource MikroTik.

---

## Minggu 12–14 : Fase Mitigasi

**Target**
- Mengurangi dampak serangan menggunakan firewall.

**Update**
- Menambahkan firewall rule pada MikroTik.
- Menerapkan pembatasan ICMP.
- Menerapkan pembatasan TCP SYN.
- Menerapkan pembatasan UDP.
- Melakukan pengujian ulang.

**Status**
✅ Firewall berhasil mengurangi dampak serangan.

**Artefak**
- Screenshot konfigurasi firewall.
- Screenshot hasil monitoring setelah hardening.

---

## Minggu 15–16 : Evaluasi

**Target**
- Mengevaluasi hasil pengujian.

**Update**
- Membandingkan kondisi sebelum dan sesudah hardening.
- Menyusun laporan akhir.
- Melakukan dokumentasi hasil proyek.

**Status**
✅ Proyek selesai.

---

# Lessons Learned

- Serangan DoS dapat mengganggu aspek availability layanan jaringan.
- Wireshark membantu proses deteksi dan analisis trafik.
- Firewall MikroTik efektif mengurangi dampak ICMP Flood, TCP SYN Flood, dan UDP Flood.
- Dokumentasi setiap tahap mempermudah proses evaluasi proyek.
