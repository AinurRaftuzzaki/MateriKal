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

  ## Eliminasi Gauss

contoh soal:
selesaikan dengan menggunakan Eliminasi Gauss

**Contoh Nomor 1**
selesaikan dengan menggunakan Eliminasi Gauss


$$\begin{array}{cc}
x_1+2x_2+3x_3=6\\
2x_1+4x_2+6x_3=12\\
x_2+x_3=2
\end{array}$$

&& Hasil Matriks: 
\begin{bmatrix}
1 & 2 & 3 & | 6 \\
2 & 4 & 6 & | 12 \\
0 & -1 & 1 & | 2
\end{bmatrix} $$

Baris kedua dikurangi 2 kali baris pertama:

$$ \begin{bmatrix}
1 & 2 & 3 & | 6 \\
0 & 0 & 0 & | 0 \\
0 & -1 & 1 & | 2
\end{bmatrix} $$

Baris kedua menjadi nol, menunjukkan bahwa sistem memiliki solusi tak hingga.
Variabel bebas: , maka

$$ x_2 = t - 2, \quad x_1 = -2x_2 - 3x_3 + 6 = -2(t-2) - 3t + 6 = -5t + 10. $$

$$ \begin{aligned}
x_1 &= -5t + 10, \\
x_2 &= t - 2, \\
x_3 &= t, \quad t \in \mathbb{R}.
\end{aligned} $$

**Contoh Nomor 2**
selesaikan dengan menggunakna Eliminasi Gauss

$$ \begin{array}{cc}
x_1+x_2+x_3=3\\
2x_1+x_3=5\\
x_1=2x_2=3\\
\end{array} $$

**Contoh Nomor 3**
selesaikan dengan menggunakna Eliminasi Gauss

$$ \begin{array}{cc}
2x_1+2x_2=4\\
x_1+x_2=2\\
\end{array} $$

$$ Hasil Matriks:
\begin{bmatrix}
2 & 2 & | Y \\
1 & 1 & | 2
\end{bmatrix} $$

Eliminasi dengan membagi baris pertama dengan 2:

$$ \begin{bmatrix}
1 & 1 & | \frac{Y}{2} \\
1 & 1 & | 2
\end{bmatrix} $$

Kurangi baris kedua dengan baris pertama:

$$ \begin{bmatrix}
1 & 1 & | \frac{Y}{2} \\
0 & 0 & | 2 - \frac{Y}{2}
\end{bmatrix} $$

Jika , baris kedua menjadi , sehingga ada solusi tak hingga:

$$ x_1 = 2 - x_2. $$

**Contoh Nomor 4**
selesaikan dengan menggunakna Eliminasi Gauss

$$ \begin{array}{cc}
x_1+x_2=5\\
x_1+2x_3=6\\
\end{array} $$

bentuk matriks:
$$ \begin{bmatrix}
   1 & 1 & 0 &|5 \\
   1 & 0 & 2 &|6
   \end{bmatrix} $$

Operasi Baris Elementer:

$$ \begin{bmatrix}
   1 & 1 & 0  &|5\\
   0 & -1 & 2 &|1
   \end{bmatrix} $$

Elemen Pivot pada Baris Kedua Menjadi 1:

$$ \begin{bmatrix}
   1 & 0 & 2  &|5\\
   0 & 1 & -2 &|-1
   \end{bmatrix} $$

Elemen di Atas Pivot pada Baris Kedua:

$$ \begin{bmatrix}
   1 & 0 & 2  &|6\\
   0 & 1 & -2 &|-1
   \end{bmatrix} $$

sistem persamaan:

$$ \begin{array}{cc}
x_1=6-2x_3\\
x_2=-1+2x_3\\
\end{array} $$