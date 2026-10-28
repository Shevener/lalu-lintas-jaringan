# Evidence dan Temuan

## Evidence 1 — Komunikasi ke IP Eksternal

Hasil analisis menunjukkan komunikasi TCP dari host internal `10.2.28.88` menuju IP eksternal `45.131.214.85` pada port 443.

Komunikasi ini menjadi indikator awal aktivitas mencurigakan yang perlu diinvestigasi.

**Bukti:** Screenshot koneksi TCP pada Wireshark.

## Evidence 2 — URI `/fakeurl.htm`

Setelah dilakukan filtering pada paket HTTP, ditemukan permintaan menuju URI `/fakeurl.htm`. Paket tersebut juga menunjukkan User-Agent `NetSupport Manager/1.3`.

Kombinasi indikator tersebut memperkuat dugaan bahwa komunikasi berkaitan dengan NetSupport RAT.

**Bukti:** Screenshot hasil filter HTTP pada Wireshark.

## Kesimpulan

Berdasarkan kedua evidence, `10.2.28.88` merupakan host yang paling kuat terindikasi menjalankan NetSupport RAT dalam PCAP yang dianalisis.

Temuan ini terbatas pada bukti jaringan yang tersedia dan belum membuktikan tindakan lanjutan seperti pencurian kredensial atau kompromi Domain Controller.
