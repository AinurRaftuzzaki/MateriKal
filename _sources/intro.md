# **Komputasi Aljabar Linier**

## **1. Pendahuluan**
Aljabar linier adalah cabang matematika yang berkaitan dengan vektor, matriks, dan sistem persamaan linier. Dalam komputasi, aljabar linier digunakan dalam berbagai bidang seperti kecerdasan buatan, grafik komputer, optimasi, dan pemrosesan sinyal.

## **2. Konsep Dasar**
### **2.1. Vektor dan Operasinya**
- Penjumlahan dan Pengurangan Vektor
- Perkalian Skalar
- Norma dan Jarak Euclidean

### **2.2. Matriks dan Operasinya**
- Penjumlahan dan Pengurangan Matriks
- Perkalian Matriks
- Determinan dan Invers Matriks

### **2.3. Sistem Persamaan Linear (SPL)**
- Representasi Matriks dari SPL
- Penyelesaian SPL dengan Eliminasi Gauss
- Penyelesaian SPL menggunakan metode Matriks Invers
- Penyelesaian SPL menggunakan **NumPy** di Python

## **3. Implementasi dalam Python**
Berikut adalah contoh implementasi beberapa operasi aljabar linier menggunakan **NumPy**:

```python
import numpy as np

# Definisi Vektor
v1 = np.array([1, 2, 3])
v2 = np.array([4, 5, 6])

# Operasi Vektor
penjumlahan = v1 + v2
perkalian_skalar = 2 * v1
norma = np.linalg.norm(v1)

print("Penjumlahan Vektor:", penjumlahan)
print("Perkalian Skalar:", perkalian_skalar)
print("Norma Vektor:", norma)

# Definisi Matriks
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])

# Operasi Matriks
perkalian_matriks = np.dot(A, B)
determinan_A = np.linalg.det(A)
invers_A = np.linalg.inv(A)

print("Perkalian Matriks:\n", perkalian_matriks)
print("Determinan A:", determinan_A)
print("Invers A:\n", invers_A)
```

## **4. Aplikasi dalam Dunia Nyata**
Aljabar linier memiliki banyak aplikasi dalam berbagai bidang seperti:
- **Pembelajaran Mesin & AI**: Representasi data, transformasi fitur, regresi linier
- **Grafik Komputer**: Transformasi 2D dan 3D
- **Optimasi**: Pemodelan linear programming
- **Pemrosesan Citra**: Filter dan transformasi gambar

## **5. Kesimpulan**
- Aljabar linier adalah dasar penting dalam komputasi modern.
- Python menyediakan pustaka seperti **NumPy** untuk melakukan perhitungan aljabar linier dengan efisien.
- Konsep seperti SPL, matriks, dan vektor memiliki banyak aplikasi praktis dalam berbagai bidang.

---