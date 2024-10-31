Berikut adalah penjelasan kode Pythonnya:

Input Data:

python
Copy code
tugas = input("Masukkan nilai Tugas: ")
uts = input("Masukkan nilai UTS: ")
uas = input("Masukkan nilai UAS: ")
Kode ini meminta pengguna untuk memasukkan nilai tugas, UTS (Ujian Tengah Semester), dan UAS (Ujian Akhir Semester).

Perhitungan Nilai Akhir:

python
Copy code
akhir = (int(tugas) * 0.2) + (int(uts) * 0.4) + (int(uas) * 0.4)
Nilai akhir dihitung berdasarkan bobot nilai tugas sebesar 20%, UTS 40%, dan UAS 40%. Fungsi int() digunakan untuk mengonversi input string menjadi integer.

Penentuan Keterangan Lulus atau Tidak:

python
Copy code
keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0]
Keterangan lulus diberikan berdasarkan nilai akhir. Jika nilai akhir lebih dari 60, maka keterangan akan menjadi "LULUS", jika tidak akan menjadi "TIDAK LULUS".

Penentuan Nilai Huruf:

python
Copy code
if akhir > 80:
    huruf = "A"
elif akhir > 70:
    huruf = "B"
elif akhir > 50:
    huruf = "C"
elif akhir > 40:
    huruf = "D"
else:
    huruf = "E"
Nilai huruf diberikan berdasarkan rentang nilai akhir:

A jika lebih dari 80
B jika lebih dari 70
C jika lebih dari 50
D jika lebih dari 40
E jika di bawah atau sama dengan 40
Output Hasil:

python
Copy code
print("\nNama :", nama)
print("Nilai UTS :", uts)
print("Nilai UAS :", uas)
print("Nilai Tugas :", tugas)
print("Nilai Akhir :", akhir)
print("Nilai Huruf :", huruf)
print("Keterangan :", keterangan)
Kode ini menampilkan hasil, termasuk nilai UTS, UAS, tugas, nilai akhir, nilai huruf, dan keterangan lulus atau tidak lulus.

Hasil Program: Pada contoh output di sisi kanan gambar, jika nilai tugas, UTS, dan UAS adalah 85, 80, dan 90, maka:

Nilai akhir adalah 85.
Nilai huruf adalah "A".
Keterangan: "LULUS".

Berikut adalah penjelasan dari kode Pythonnya:

Input Data:

python
Copy code
gaji = int(input("Masukkan gaji: "))
berkeluarga = (False, True)[input("Sudah berkeluarga? (Y/T) ") == "Y"]
punya_rumah = (False, True)[input("Punya rumah? (Y/T) ") == "Y"]
Kode ini meminta pengguna untuk memasukkan gaji, status keluarga, dan kepemilikan rumah.
Variabel gaji menyimpan nilai gaji sebagai integer.
Variabel berkeluarga akan bernilai True jika pengguna memasukkan "Y" (sudah berkeluarga) dan False jika "T".
Variabel punya_rumah akan bernilai True jika pengguna memasukkan "Y" (punya rumah) dan False jika "T".
Pengecekan Gaji:

python
Copy code
if gaji > 3000000:
    print("Gaji sudah di atas UMR")
Jika gaji lebih dari 3.000.000, maka program akan mencetak "Gaji sudah di atas UMR". Jika tidak, program akan langsung mencetak "Gaji belum UMR" pada bagian else.

Pengecekan Status Keluarga:

python
Copy code
if berkeluarga:
    print("Wajib ikutan asuransi dan menabung untuk pensiun")
else:
    print("Tidak perlu ikutan asuransi")
Jika berkeluarga bernilai True, program akan menampilkan "Wajib ikutan asuransi dan menabung untuk pensiun".
Jika berkeluarga bernilai False, program akan menampilkan "Tidak perlu ikutan asuransi".
Pengecekan Kepemilikan Rumah:

python
Copy code
if punya_rumah:
    print("Wajib bayar pajak rumah")
else:
    print("Tidak wajib bayar pajak rumah")
Jika punya_rumah bernilai True, program akan menampilkan "Wajib bayar pajak rumah".
Jika punya_rumah bernilai False, program akan menampilkan "Tidak wajib bayar pajak rumah".
Gaji di Bawah UMR:

python
Copy code
else:
    print("Gaji belum UMR")
Jika gaji tidak lebih dari 3.000.000, program akan langsung menampilkan "Gaji belum UMR" tanpa melakukan pengecekan tambahan.

Hasil Program: Pada contoh output di sisi kanan gambar, jika gaji 4.000.000, status berkeluarga "Y", dan punya rumah "Y":

Program menampilkan bahwa gaji di atas UMR.
Menampilkan bahwa pengguna wajib ikut asuransi dan menabung untuk pensiun.
Menampilkan bahwa pengguna wajib membayar pajak rumah.

Berikut adalah penjelasan kode Pythonnya:

Input Data:

python
Copy code
a = int(input("Masukkan bilangan A: "))
b = int(input("Masukkan bilangan B: "))
c = int(input("Masukkan bilangan C: "))
Kode ini meminta pengguna untuk memasukkan tiga bilangan: a, b, dan c.
Input dari pengguna dikonversi ke tipe int agar dapat digunakan dalam operasi aritmatika.
Pengecekan Kondisi:

python
Copy code
if a + b == c or b + c == a or c + a == b:
    print("BENAR")
else:
    print("SALAH")
Kode ini memeriksa apakah salah satu dari kondisi berikut terpenuhi:
a + b == c
b + c == a
c + a == b
Jika salah satu kondisi di atas benar, program akan mencetak "BENAR".
Jika tidak ada kondisi yang terpenuhi, program akan mencetak "SALAH".
Penjelasan Logika:

Kode ini mengecek apakah salah satu dari tiga bilangan (a, b, atau c) dapat merupakan hasil penjumlahan dari dua bilangan lainnya.
Pada contoh output di sebelah kanan gambar:
Jika a = 100, b = 50, dan c = 200, maka tidak ada kondisi yang terpenuhi, sehingga hasilnya adalah "SALAH".

Kode Python di atas adalah program untuk menghitung total harga tiket bioskop. Program ini meminta input dari user untuk tipe tiket (reguler atau VIP) dan status member (memiliki kartu member atau tidak).

Berikut adalah langkah-langkah program:

Mendefinisikan harga tiket:

harga_tiket_reguler: Harga tiket reguler didefinisikan sebesar 50000
harga_tiket_vip: Harga tiket VIP didefinisikan sebesar 100000
diskon_member: Besar diskon untuk member didefinisikan sebesar 0.20 (20%)
Meminta input dari user:

Program meminta user untuk memasukkan tipe tiket (reguler/vip) dan menyimpannya ke dalam variabel tipe_tiket.
Program meminta user untuk memasukkan status member (ya/tidak) dan menyimpannya ke dalam variabel status_member.
Kedua input dari user diubah menjadi huruf kecil menggunakan fungsi lower().
Menghitung harga tiket berdasarkan tipe:

Program memeriksa nilai tipe_tiket:
Jika tipe_tiket adalah "reguler", maka harga_tiket diset menjadi harga_tiket_reguler.
Jika tipe_tiket adalah "vip", maka harga_tiket diset menjadi harga_tiket_vip.
Jika tipe_tiket bukan "reguler" atau "vip", maka program menampilkan pesan "Tipe tiket tidak valid" dan keluar dari program.
Mengecek status member untuk diskon:

Program memeriksa nilai status_member:
Jika status_member adalah "ya", maka total_harga dihitung dengan rumus harga_tiket * (1 - diskon_member), yang memberikan diskon kepada member.
Jika status_member bukan "ya", maka total_harga diset sama dengan harga_tiket tanpa diskon.
Menampilkan total harga yang harus dibayar:

Program menampilkan total harga yang harus dibayar dengan format "Total harga yang harus dibayar: Rp(total_harga)" menggunakan fungsi print().

Kode program ini dirancang untuk melakukan operasi aritmatika sederhana berdasarkan input pengguna. Berikut penjelasan kode secara detail:

Input: Kode program meminta pengguna untuk memasukkan operator aritmatika (+, -, *, /) dan dua angka.
Validasi Operator: Kode menggunakan struktur if-elif-else untuk memvalidasi operator yang dimasukkan.
Operasi Aritmatika: Berdasarkan operator yang valid, kode melakukan operasi aritmatika yang sesuai dan menyimpan hasilnya dalam variabel hasil.
Validasi Pembagian dengan Nol: Kode mengecek apakah angka kedua adalah nol untuk menghindari pembagian dengan nol. Jika angka kedua nol, program akan menampilkan pesan error dan menghentikan eksekusi.
Output: Jika operator valid dan operasi berhasil dilakukan, kode mencetak hasil perhitungan ke layar. Jika operator tidak valid atau terjadi pembagian dengan nol, kode mencetak pesan error.
Secara keseluruhan, kode ini mengilustrasikan penggunaan struktur kontrol if-elif-else untuk membuat program sederhana yang dapat melakukan operasi aritmatika dasar.
