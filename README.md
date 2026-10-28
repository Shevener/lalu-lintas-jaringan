# lalu-lintas-jaringan

 Berdasarkan bukti jaringan, host kemungkinan memiliki akses RAT aktif dengan kemampuan
 umum NetSupport Manager, seperti:

 - Remote command execution
 - Pengambilan informasi host
 - File transfer
 - Remote desktop/control
 - Persistence
 - Credential theft atau abuse terhadap kredensial yang tersedia
 - Penggunaan host untuk aktivitas lanjutan dalam jaringan

 Karena host memiliki koneksi ke Domain Controller menggunakan SMB, LDAP, Kerberos, dan
 RPC, kemungkinan risiko meliputi:

 - Penyalahgunaan kredensial domain
 - Pengumpulan informasi AD
 - Akses ke shared folder
 - Lateral movement
 - Penyebaran malware
 - Akses terhadap resource domain

 Pcap tidak memberikan bukti yang cukup untuk memastikan apakah data berhasil
 dieksfiltrasi atau apakah command tertentu telah dijalankan.
