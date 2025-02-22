# Definisi Sistem Persamaan Linier

## **1. Definisi Persamaan Linear**

Persamaan linear dalam *n* variabel (*unknown*, *anu*) \(x_1, x_2, ..., x_n\) adalah persamaan yang memiliki bentuk umum:

\[
a_1 x_1 + a_2 x_2 + ... + a_n x_n = b
\]

dengan \(a_1, a_2, ..., a_n, b\) merupakan bilangan real, dan tidak semua \(a_i\) untuk \(i = 1, 2, ..., n\) adalah nol.

- **Koefisien**: Setiap bilangan \(a_i\) disebut sebagai koefisien variabel \(x_i\).
- **Suku Konstan**: Bilangan \(b\) disebut sebagai suku konstan.

## **2. Contoh Sistem Persamaan Linear**
Sistem persamaan linear terdiri dari beberapa persamaan linear yang melibatkan beberapa variabel. Berikut adalah contoh sistem persamaan linear dengan dua variabel:

\[
\begin{cases}
2x + 3y = 8 \\
5x - y = 3
\end{cases}
\]

Pada contoh di atas:
- \(a_1 = 2, a_2 = 3, b = 8\) untuk persamaan pertama.
- \(a_1 = 5, a_2 = -1, b = 3\) untuk persamaan kedua.

Sistem ini dapat diselesaikan dengan berbagai metode seperti **substitusi, eliminasi, matriks**, atau metode numerik lainnya.

## **3. Implementasi dalam Python**
Berikut adalah contoh kode Python untuk menyelesaikan sistem persamaan linear menggunakan **NumPy**:

```python
import numpy as np

# Matriks koefisien
A = np.array([[2, 3], [5, -1]])
# Vektor hasil
B = np.array([8, 3])

# Menyelesaikan sistem persamaan
X = np.linalg.solve(A, B)
print("Solusi: x =", X[0], ", y =", X[1])
```

Kode di atas menggunakan `numpy.linalg.solve()` untuk menemukan solusi dari sistem persamaan linear secara langsung.

## **4. Kesimpulan**
- **Persamaan linear** adalah persamaan yang memiliki variabel dengan pangkat satu.
- **Sistem persamaan linear** terdiri dari beberapa persamaan linear dengan beberapa variabel.
- **Metode penyelesaian** dapat menggunakan metode aljabar seperti substitusi dan eliminasi, atau metode berbasis matriks dengan pemrograman.
- **Python (NumPy)** dapat digunakan untuk menyelesaikan SPL dengan efisien.

Dokumentasi ini dapat digunakan sebagai referensi dasar untuk memahami sistem persamaan linear dan implementasinya dalam pemrograman.