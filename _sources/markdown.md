# Definisi Sistem Persamaan Linier

## **1. Definisi Persamaan Linear**

Persamaan ini disebut linear lantaran hubungan matematis ini dapat digambarkan sebagai garis lurus dalam sistem koordinat kartesius. Apabila terdapat lebih dari satu persamaan linear, persamaan tersebut akan menjadi sebuah sistem.
Bentuk umum untuk persamaan linear adalah: 

y = mx + b 

## **2. Sistem Persamaan Linear Satu Variabel

Dalam sistem persamaan ini hanya terdapat sebuah variabel saja berpangkat satu. Adapun bentuk umumnya, yakni: 

ax + b = 0.

a dan b adalah bilangan bulat bukan nol dan b konstanta.

Di mana:
- `a` dan `b` adalah konstanta
- `x` adalah variabel
- `a ≠ 0`

## Contoh
Berikut adalah contoh persamaan linier satu variabel:

```
2x - 5 = 0
```

Untuk menyelesaikan persamaan ini, kita mencari nilai `x`:

```
2x - 5 = 0
2x = 5
x = 5/

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