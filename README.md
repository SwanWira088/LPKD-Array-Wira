## 1. Mengapa Kita Memerlukan Array?
Array digunakan untuk **menyimpan banyak data dalam satu variabel**.  
Tanpa array, kita harus membuat banyak variabel satu per satu.

**Contoh tanpa array:**
```js
let nilai1 = 80;
let nilai2 = 90;
let nilai3 = 85;
```

**Contoh dengan array:**
```js
let nilai = [80, 90, 85];
```
## 2. Bagaimana Array Menghemat Variabel
Array menghemat variabel karena **semua data disimpan dalam satu wadah**.

Misalnya kamu punya 100 nilai siswa:  
Tanpa array, kamu butuh 100 variabel.  
Dengan array, cukup satu:
```js
let nilaiSiswa = [80, 90, 70, 85, 95];
```
## 3. Apa Dampak Data Bertambah pada Array
Jika data dalam array bertambah:
- Ukuran array **bertambah otomatis**.
- **Akses data bisa sedikit lebih lambat** jika datanya sangat besar.
- Tapi umumnya tidak masalah karena array sudah dioptimalkan oleh JavaScript.

**Contoh:**
```js
let angka = [1, 2, 3];
angka.push(4);
console.log(angka); // [1, 2, 3, 4]
```

## 4. Strategi Menampilkan Data Tertentu
Gunakan **indeks**, **looping**, atau **metode array** seperti `filter`, `find`, dan `map`.

**Dengan indeks:**
```js
console.log(nilai[1]); // tampilkan elemen ke-2
```
**Dengan find:**
```js
let nilaiPertama90 = nilai.find(n => n === 90);
```
**Dengan filter:**
```js
let tinggi = nilai.filter(n => n > 85);
console.log(tinggi); // nilai di atas 85
```

## 5. Kesalahan Umum dalam Penggunaan Array
Beberapa kesalahan yang sering terjadi:

1. **Salah indeks**
   ```js
   console.log(nilai[10]); // undefined
   ```
2. **mengunakan lebi dari satu tipe data**
   ```js
   let data = [90, "A", true]; // bisa, tapi membingungkan
   ```
3. **lupa jika indeks itu mulai nya dari 0**
4. **tidak memakai metode yg udh disediakan oleh js**
