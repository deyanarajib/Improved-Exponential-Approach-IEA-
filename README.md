# Improved-Exponential-Approach-IEA-
A method for solving Transportation Problem

Algoritma Improved Exponential Approach (IND)
Langkah 1: Membentuk model transportasi (Tabel) dari masalah transportasi yang diberikan. Apabila tabel transportasi belum seimbang ke langkah 2, jika sudah seimbang langsung ke langkah 3.
Langkah 2: Jika kolom (baris) dummy ditambahkan, kurangi setiap entri kolom (baris) dari minimum kolom (baris) masing-masing. Mengganti biaya dummy dengan biaya yang terbesar dari tabel yang sudah direduksi sebelumnya. Jika kolom dummy yang ditambahkan maka ke step 3a lalu 3b dan jika baris dummy yang ditambahkan maka ke step 3b lalu 3a.
Langkeh 3:
	a. Mengurangi setiap entri baris dari tabel transportasi dari minimum baris masing-masing.
	b. Mengurangi setiap entri kolom tabel transportasi dari kolom minimum masing-masing. Sehingga setiap baris dan kolom akan memiliki setidaknya satu nol.
Langkah 4: Mengecek apakah setiap kolom permintaan kurang dari atau sama dengan jumlah persediaan dalam baris dengan melihat pada kolom yang biaya tereduksinya bernilai nol. Mengecek apakah setiap baris persediaan kurang dari atau sama dengan jumlah permintaan dalam kolom dengan melihat pada baris yang biaya tereduksinya bernilai nol. Apabila syarat tersebut terpenuhi langsung ke langkah 7. Jika tidak, lanjut ke langkah 5.
Langkeh 5: Menarik garis horisontal dan vertikal pada semua baris dan kolom yang memiliki angka nol dengan jumlah garis minimum, sedemikian hingga biaya yang tidak memenuhi pada langkah 4 tidak tertutup.
Langkeh 6: Memilih biaya terkecil pada sel yang tidak terkena garis, kemudian mengurangkan sebesar biaya terpilih ke semua biaya yang tidak terkena garis. Menambahkan sebesar biaya terpilih ke semua biaya yang terletak pada perpotongan dua garis. Kembali ke langkah 4.
Langkeh 7: Memilih nol yang terdapat dalam tabel. Menghitung jumlah total angka nol (tidak termasuk yang dipilih) dalam baris dan kolom yang bersesuaian. Menetapkan penalti eksponen (jumlah nol berturut-turut masing-masing baris dan kolom). Mengulangi prosedur diatas untuk semua nol dalam tabel.
Langkeh 8: Mengalokasikan nilai sel dengan jumlah maksimum yang mungkin dengan memperhatikan prioritas pengalokasian sebagai berikut:
	a. Nol yang memiliki penalti eksponen bernilai 0.
	b. Nol yang memiliki penalti eksponen bernilai 1.
	c. Memilih sel yang memiliki biaya tereduksi terbesar dan dinamakan ( ). Jika terdapat lebih dari satu sel, maka memilih sel lain dengan biaya tereduksi terbesar berikutnya. Mengalokasikan pada nol yang terdapat pada baris i atau kolom j dengan penalti eksponen yang minimum hingga persediaan baris i atau permintaan kolom j terpenuhi.
	d. Memilih nol dengan penalti eksponen minimum pada tabel. Jika terjadi nilai penalti eksponen sama untuk setiap sel maka pertama memeriksa nilai permintaan dan persediaan, menghitung nilai rata-ratanya dan menetapkan alokasi untuk nilai rata-rata terendah. Apabila tetap sama maka mengalokasikan pada sel dengan biaya yang terendah sebelum direduksi.
Langkeh 9: Menandai baris atau kolom (di mana persediaan atau permintaan menjadi nol) untuk tidak dimasukan dalam perhitungan selanjutnya, kemudian kembali ke langkah 4 hingga semua permintaan dan persediaan terpenuhi.
Langkeh 10: Menghitung biaya optimumnya.

Sumber: Dimas Alfan Hidayat, Siti Khabibah, dan Suryoto, "Metode Improved Exponential Approach dalam Menentukan Solusi Optimum pada Masalah Transportasi", Universitas Diponegoro.
