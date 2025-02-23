# **Eliminasi Persamaan Linier**
Penyelesaian SPLDV menggunakan model eliminasi adalah dengan menghapus atau menghilangkan salah satu variabel dalam persamaan tersebut. Dalam sistem persamaan linier, terdapat beberapa metode eliminasi yang digunakan untuk menyelesaikan sistem persamaan tersebut.

## Metode Eliminasi Substitusi

- alah satu variabel diisolasi dalam satu persamaan.
- Hasil isolasi variabel tersebut kemudian disubstitusikan ke persamaan lainnya.
- Proses ini diulang sampai diperoleh nilai semua variabel.

**Contoh:**
```math
2x + y = 8
x - y = 2
```
**Langkah-langkah:**
1. Isolasi salah satu variabel dari persamaan kedua:
   ```math
   x = y + 2
   ```
2. Substitusikan ke persamaan pertama:
   ```math
   2(y + 2) + y = 8
   2y + 4 + y = 8
   3y = 4
   y = 4/3
   ```
3. Substitusikan kembali nilai `y`:
   ```math
   x = 4/3 + 2 = 10/3
   ```
**Hasil:**
```math
x = 10/3, y = 4/3
  ```

## Metode Eliminasi Gauss

- Mengubah sistem persamaan linier menjadi bentuk segitiga atas dengan menggunakan operasi baris dasar.
- Setelah diperoleh bentuk segitiga atas, solusi dapat ditemukan dengan substitusi mundur (back-substitution).

**Contoh:**
```math
x + 2y + 3z = 9
2x + 3y + z = 4
3x + y + 2z = 10
```
**Matriks Augmented:**
```math
 |1 2 3 9 |
 |2 3 1 4 |
 |3 1 2 10|
```
**Langkah-langkah:**
1. Eliminasi `x`:
```math
 |1   2   3   9 |
 |0  -1  -5 -14 |
 |0  -5  -7 -17 |
```
2. Eliminasi `y`:
```math
 |1  2  3    9 |
 |0 -1 -5  -14 |
 |0  0 -32 -87 |
```
3. Substitusi mundur:
```math
z = -͟3͟2͟ = 3͟2͟
    −87   87
  ```

## Metode Eliminasi Gauss-Jordan

- Merupakan penyempurnaan dari metode eliminasi Gauss.
- Mengubah sistem persamaan menjadi bentuk matriks eselon baris tereduksi (Reduced Row Echelon Form, RREF).
- Penyelesaian diperoleh langsung tanpa perlu substitusi mundur.

  ```math
  2x + 3y = 6
  x - y = 2
  ```

## Metode Eliminasi Matriks (Invers Matriks)

- Jika sistem persamaan dapat dituliskan dalam bentuk matriks AX = B, maka solusi dapat ditemukan dengan X = A⁻¹B, asalkan matriks A memiliki invers.

  ```math
  2x + 3y = 6
  x - y = 2
  ```