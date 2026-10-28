Analisis Network Traffic — NetSupport RAT

Analisis dilakukan terhadap file PCAP menggunakan TShark dan Wireshark untuk mengidentifikasi komunikasi jaringan yang mencurigakan.

Dari hasil analisis, ditemukan bahwa host internal `10.2.28.88` berkomunikasi dengan IP eksternal `45.131.214.85` melalui TCP port 443. Komunikasi tersebut menggunakan URI `/fakeurl.htm` dan User-Agent `NetSupport Manager/1.3`, yang mengindikasikan aktivitas terkait NetSupport RAT.

HASIL IDENTIFIKASI

- **IP internal:** `10.2.28.88`
- **Hostname:** `DESKTOP-TEYQ2NR`
- **IP eksternal:** `45.131.214.85`
- **Port tujuan:** TCP 443
- **URI mencurigakan:** `/fakeurl.htm`
- **User-Agent:** `NetSupport Manager/1.3`

EVIDENCE

1. Komunikasi TCP antara `10.2.28.88` dan `45.131.214.85` pada port 443.
2. Permintaan HTTP yang menunjukkan URI `/fakeurl.htm`.

## Kesimpulan

Berdasarkan bukti komunikasi jaringan dan indikator NetSupport Manager yang ditemukan, host `10.2.28.88` diduga terinfeksi atau menjalankan NetSupport RAT. Pemeriksaan lebih lanjut diperlukan untuk memastikan dampak infeksi.
