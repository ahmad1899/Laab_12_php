# Lab12Web

<Hr>

|NAMA   |ACHMAD SYARIFUDIN |
| --- | --- |
| NIM   | 312110598 |
| KELAS | TI.21.B1 |
| DOSEN | Agung Nugroho,S.Kom.,M.Kom |
| Matkul| Pemograman web |
|Pertemuan| KE 14 |
|Kampus | UNIVERSITAS PELITA BANGSA |

<Hr>

## Membuat Pencarian Data
Untuk membuat pencarian data, yang perlu di perhatikan adalah penggunaan filter pada query data.
<br>
Pada data awal, query untuk menampilkan semua data adalah:
<br>
$sql = “SELECT * FROM data_barang”;

<br>

Nah untuk menambahkan pencarian, maka query tersebut harus ditambahkan klausa WHERE sebagai filter, sehingga menjadi:
<br>
$sql = “SELECT * FROM data_barang WHERE nama = ‘{$var_nama}’”;
<br>
Atau dapat juga menggunakan LIKE seperti berikut:
<br>
$sql = “SELECT * FROM data_barang WHERE nama LIKE ‘{$var_nama}%’”;
<br>

Langkah-langkah buat form pencarian
![gambar1](https://imgur.com/7YvYbHO.png)
Sisipkan kode tersebut pada file index.php (daftar barang), sebelum table data dan sesudah tombol tambah data. <br>
Lalu rubah querynya dan tambahkan filter pencarian pada query tersebut.
![gambar2](https://imgur.com/inLp7ot.png)
Maka Hasilnya akan seperti ini
![gambar2](https://imgur.com/lazU65O.png)
