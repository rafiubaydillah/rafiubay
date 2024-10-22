# rafiubay
![flowchart](<gambar flowchr.jpg>)
















1.	  Mulai (Start).
2.	 Inisialisasi max = -∞.
3.	Input bilangan N.
4.	Apakah N = 0?
•	Jika Ya, cetak max dan lanjutkan ke Selesai.
•	Jika Tidak, lanjut ke langkah berikutnya.
5.	Apakah N > max?
•	Jika Ya, set max = N.
•	Jika Tidak, lanjutkan ke langkah berikutnya.
6.	Kembali ke langkah 3 (input bilangan berikutnya).
7.	 Jika input adalah 0, cetak max.
8.	Selesai (End).

# Inisialisasi variabel max untuk menyimpan bilangan terbesar
max_number = float('-inf')  # Menggunakan nilai -∞ agar setiap bilangan positif bisa lebih besar

while True:
    # Input bilangan dari pengguna
    N = float(input("Masukkan bilangan (masukkan 0 untuk berhenti): "))
    
    # Periksa apakah input adalah 0
    if N == 0:
        break  # Keluar dari loop jika input 0
    
    # Bandingkan bilangan yang diinputkan dengan max_number
    if N > max_number:
        max_number = N  # Jika bilangan lebih besar, update max_number

# Tampilkan bilangan terbesar
if max_number == float('-inf'):
    print("Tidak ada bilangan yang diinput.")
else:
    print(f"Bilangan terbesar yang diinputkan adalah: {max_number}")
