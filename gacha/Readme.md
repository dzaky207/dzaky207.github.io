# Slot Simulation Control System

## Disclaimer

Proyek ini dibuat **hanya untuk keperluan simulasi dan edukasi**.  
Bukan sistem perjudian nyata dan tidak terhubung dengan transaksi uang asli, namun ini mensimulasikan kasus nyata.

Sistem ini mensimulasikan mekanisme slot (sering disebut "judol") di mana:
- Admin dapat mengatur peluang kemenangan user.
- User hanya melakukan percobaan simulasi di link yang diberikan admin.

Tujuan utama proyek ini adalah demonstrasi logika sistem, pengaturan probabilitas, dan kontrol mekanisme jackpot.

## Deskripsi

- **remote.html** → File UI untuk mengatur preset / konfigurasi kemenangan gacha.  
- **gacha.html** → Halaman untuk melakukan gacha. Jika dibuka langsung tanpa pengaturan, persentase menang default adalah **15%**.

---

## Cara Penggunaan

1. Buka `remote.html`.
2. Salin link pada kolom **Room Aktif**. Link tersebut adalah halaman gacha yang bisa dikontrol persentase menangnya.
3. Pilih mode jackpot yang ingin digunakan:

   - **Persentase**  
     Mengatur peluang jackpot secara langsung (1%–100%).

   - **Guaranteed**  
     Sistem pity. Jackpot akan diberikan setelah **N** kali percobaan jika belum mendapatkannya.  
     Selama periode tersebut, peluang jackpot tetap berjalan normal. Nilai **N** dapat disesuaikan.

   - **Terkunci**  
     Jackpot tidak bisa didapatkan sampai **N** kali percobaan terpenuhi. Nilai **N** dapat disesuaikan.

   - **Nonaktif**  
     Jackpot tidak bisa didapatkan sama sekali.

4. Alternatifnya, gunakan preset cepat yang tersedia.
5. Klik **“Terapkan ke Room Ini”**.
6. Buka link **Room Aktif** di tab baru.
7. Voila! gacha di link tersebut sudah disetting
