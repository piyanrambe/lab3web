# lab3web
### Disini saya akan menjelaskan langkah langkah Praktikum ke 3
### berikut adalah urutan langkah langkah yang akan saya jelaskan
### 1. Membuat LIST pada HTML
### 2. Membuat TABLE pada HTML
### 3. Membuat FORM pada HTML
============================================================================================

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
============================================================================================

# B. Membuat Tabel dan menggabungkan Sel data di HTML
Disini saya akan menjelaskan cara membuat Tabel.
### 1. Pertama adalah cara memmbuat tabel di HTML
ada beberapa element yang digunakan khusus untuk membuat tabel, contohnya :
- element `<table></table>` yang berguna unutk mendefinisikan sebuah tabel dalam dokumen HTML.
- element `<th></th>` yang berguna membuat judul pada kolom atas
- element `<tr></tr>` untuk mendefinisikan baris dalam tabel
- element `<td></td>` untuk mendefinisikan kolom tabel

berikut adalah hasil dari membuat tabel beserta code nya :
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML Lanjutan</title>
  </head>
  <body>
    <!-- Membuat table -->
    <h1>Membuat Tabel</h1>
    <table border="1" cellpadding="4" cellspacing="0">
      <!-- table header -->
      <thead>
        <tr>
          <th>No.</th>
          <th>Fakultas</th>
          <th>Program Studi</th>
        </tr>
      </thead>
      <!-- table body -->
      <tbody>
        <tr>
          <td>1.</td>
          <td>Teknik</td>
          <td>Teknik Informatika</td>
        </tr>
        <tr>
          <td>2.</td>
          <td>Teknik</td>
          <td>Teknik Industri</td>
        </tr>
        <tr>
          <td>3.</td>
          <td>Teknik</td>
          <td>Teknik Lingkungan</td>
        </tr>
      </tbody>
    </table>
    <br>
```
![4 membuat tabel](https://user-images.githubusercontent.com/101393632/159869719-c661427c-cef7-4e49-9472-8c0d1b740aeb.jpg)

### 2. menggabungkan Cell data.
ada dua atribut dalam element `<table>` yaitu : 
- `colspan` berguna untuk menggabungkan beberapa cell dalam satu baris
- `rowspan` berguna untuk menggabungkan beberapa cell dalam satu kolom

Cara menggunakannya yaitu `<td rowspan="3">Teknik</td>`

dan dibawah ini adalah code untuk penggabungan Cell Data : 
```
<table border="1" cellpadding="6" cellspacing="0">
      <thead>
        <tr>
          <th>No.</th>
          <th>Fakultas</th>
          <th>Program Studi</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1.</td>
          <td rowspan="3">Teknik</td>
          <td>Teknik Informatika</td>
        </tr>
        <tr>
          <td>2.</td>
          <td>Teknik Industri</td>
        </tr>
        <tr>
          <td>3.</td>
          <td>Teknik Lingkungan</td>
        </tr>
      </tbody>
    </table>
  </body>
</html>
```
![5 menggabungkan sel data](https://user-images.githubusercontent.com/101393632/159870992-c8138457-d2b7-4313-93aa-e43ff9b9d430.jpg)
============================================================================================

# C. Membuat Form 
cara membuat Form harus menggunakan tag `<form></form>`, karena tag ini akan membungkus element input yang ada dialamanya dan juga berfungsi mengirim data ke server.
contoh element yang berada di dalam tag tersebut adalah :
- `<textfield>`
- `<password>`
- `<checkbox>`
- `<Radio>`
- `dll`

Dibawah ini adalah code pembuatan Form sesuai praktikum 3 : 
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML Lanjutan</title>
  </head>
  <body>
    <!-- Membuat Form -->
    <h1>Membuat Form</h1>
    <form action="#" method="post">
      <fieldset>
        <legend>Data Pelanggan</legend>
        <div>
          <label for="nama">Nama</label>
          <input type="text" id="nama" name="nama" />
        </div>
        <div>
          <label for="alamat">Alamat</label>
          <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
        </div>
        <!-- membuat label input radio -->
        <div>
          <label>Jenis Kelamin</label>
          <input id="jk_l" type="radio" name="kelamin" value="L" />
          <label for="jk_l"> Laki-laki </label>
          <input id="jk_p" type="radio" name="kelamin" value="P" />
          <label for="jk_p"> Perempuan </label>
        </div>
        <div><input type="submit" value="Login" /></div>
       </fieldset>
    </form>
  </body>
</html>
```
![6 membuat Form](https://user-images.githubusercontent.com/101393632/159877811-46fee145-f81b-41d7-8b11-4548f51c0086.jpg)

### menambah Style Pada Form
agar tampilan lebih menarik, kita akan tambahkan seditik style di form ini. untuk element `<style>`, kita akan taruh di antara tag `<head>` dan `</head>`
berikut codenya :
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML Lanjutan</title>

    <!-- Menambah Style -->
    <style>
      form div {
        margin: 0.8rem 0rem;
      }
      form div > label {
        display: inline-block;
        width: 100px;
      }
      form input[type="text"],
      form textarea {
        border: 1px solid #197a43;
      }
      form input[type="submit"] {
        border: 1px solid #197a43;
        background-color: #197a43;
        color: #ffffff;
        font-weight: bold;
        padding: 5px 15px;
      }
      select {
        border: 1px solid #197a43;
        
      }
    </style>
  </head>
```
![7 menambah Style pada form](https://user-images.githubusercontent.com/101393632/159878346-4fe5cffa-2038-4bc8-9229-01733292fab9.jpg)
============================================================================================

# Pertanyaan dan tugas
## Buatlah form yang menampilkan **dropdown** menu dan **listbox** dengan multiple selection.

Disini saya menambahkan elemen `<option>` untuk menu **Dropdown**, Berikut Code nya :
```
<div>
          <label for="Asal kota">Asal Kota</label>
          <select>
            <option selected>--pilih kota asal--</option>
            <option>Cikarang</option>
            <option>Jakarta</option>
            <option>Karawang</option>
            <option>Bekasi</option>
            <option>Subang</option>
          </select>
</div>
```
Dan dibawah ini akan saya tampilkan **listbox** multiple selection.

disini saya menggunakan element `<input type="Checkbox">`, berikut codenya :
```
 <div>
          <label for="Hobi">Pilih Hobi</label>
          <input type="checkbox" name="Hobi" value="Olahraga"><label>Olahraga</label>
          <input type="checkbox" name="Hobi" value="Membaca"><label>Membaca</label>
          <input type="checkbox" name="Hobi" value="Memancing"><label>Memancing</label>
          <input type="checkbox" name="Hobi" value="Musik"><label>Musik</label>
 </div>
```
Berikut Hasilnya
![8 menambah dropdown dan listbox](https://user-images.githubusercontent.com/101393632/159879748-51144fff-27d2-4790-be49-c0297d7fca11.jpg)

## **Alfiansyah Rambe - 312010338 - TI 20 B2**
======================================SELESAI===============================================



