# lab3web
### Disini saya akan menjelaskan langkah langkah Praktikum ke 3
===================================================================

# A. Membuat LIST di HTML
### 1. Ordered List
Disini saya menggunakan text editor VS Code. lalu yang pertama kita harus lakukan adalah membuat file html dengan nama **lab3_list.html**.
Setelah itu masukan code seperti dibawah ini :
```
<section id="order-list">
      <h2>Ordered List</h2>
      <ol>
        <li>Pemrograman Web</li>
        <li>Sistem Informasi</li>
        <li>Basis Data 2</li>
      </ol>
    </section>
```
![1 menambah ordered list](https://user-images.githubusercontent.com/101393632/159863811-0e8939d8-965b-4769-b3cd-2a33892e2405.jpg)

### 2. Unordered List
setelah membuat ordered list seperti di atas, kita lanjutkan dengan membuat Unordered list. tampilan code seperti dibawah ini :
```
<section id="unorder-list">
      <h2>Unordered List</h2>
      <ul type="square">
        <li>Jaringan Komputer</li>
        <li>Struktur Data</li>
        <li>Algoritma &amp; Pemrograman</li>
      </ul>
    </section>

```
![2 unordered List](https://user-images.githubusercontent.com/101393632/159864174-a12cb2f9-194c-48d9-b27e-f13889897410.jpg)

### 3. Description List
Cara membuat **Description List**, ikuti saja kode dibawah ini :
```
<section id="description-list">
      <h2>Description List</h2>
      <dl>
        <dt>Fakultas Teknik</dt>
        <dd>Teknik Industri</dd>
        <dd>Teknik Informatika</dd>
        <dd>Teknik Lingkungan</dd>
        <dt>Fakultas Ekonomi dan Bisnis</dt>
        <dd>Akuntansi</dd>
        <dd>Manajemen</dd>
        <dd>Bisnis Digital</dd>
      </dl>
    </section>
```
![3 menambah description list](https://user-images.githubusercontent.com/101393632/159865587-c2deb79f-4503-489b-a3a2-bf8920ffbc76.jpg)

# B. Membuat Tabel dan menggabungkan Sel data di HTML
Disini saya akan menjelaskan cara membuat Tabel.
### 1. Pertama adalah cara memmbuat tabel di HTML
ada beberapa element yang digunakan khusus untuk membuat tabel, contohnya :
- element `<table></table>` yang berguna unutk mendefinisikan sebuah tabel dalam dokumen HTML.
- element `<th></th>` yang berguna membuat judul pada kolom atas
- element `<tr></tr>` untuk mendefinisikan baris dalam tabel
- element `<td></td>` untuk mendefinisikan kolom tabel

