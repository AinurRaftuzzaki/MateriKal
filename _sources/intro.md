# Sistem Persamaan Linier
# **Sistem Persamaan Linear (SPL)**

## **1. Konsep Sistem Persamaan Linear (SPL)**
Sistem persamaan linear (SPL) mencakup definisi, jenis-jenis SPL, dan metode penyelesaiannya.

**Video terkait materi ini dapat diakses dengan cara memindai kode di bawah ini.**

## **2. Aplikasi SPL dalam Kehidupan Sehari-hari**
Banyak permasalahan nyata yang dapat dimodelkan menggunakan SPL, di antaranya:

1. **Masalah Harga Barang di Koperasi**
   - Siswa A membeli 3 buku tulis dan 2 pulpen seharga Rp22.000,-.
   - Siswa B membeli 2 buku tulis dan 2 pulpen seharga Rp16.000,-.
   - Berapa harga satuan buku tulis dan pulpen?
```

2. **Masalah Perjalanan Pesawat**
   - Pesawat P1 menempuh perjalanan 1.500 km selama 2,5 jam dengan arah angin.
   - Pesawat P2 menempuh perjalanan yang sama selama 3 jam melawan arah angin.
   - Tentukan kecepatan pesawat dan kecepatan angin.
```

3. **Masalah Perpotongan Garis**
   - Diberikan dua persamaan garis: 
     \[ 3x + 2y = 10 \] 
     \[ 3x + 2y = 25 \]
   - Apakah kedua garis berpotongan? Jika ya, tentukan titik potongnya.
```

4. **Masalah Tiket Pameran**
   - Tiket anak-anak: Rp20.000,00
   - Tiket dewasa: Rp35.000,00
   - Terdapat 1.400 pengunjung dengan total pendapatan Rp43.000.000,00.
   - Tentukan jumlah pengunjung anak-anak dan dewasa.
```

5. **Masalah Bilangan Tiga Digit**
   - Bilangan tiga digit \(zyz\) dengan digit \(x, y, z\) memenuhi:
     \[ x + y + z = 10 \]
   - Jika urutan digit dibalik, nilainya berkurang 99.
   - Tentukan semua kemungkinan bilangan tersebut.

## **3. Model Matematika dan Penyelesaian SPL**
Setiap permasalahan di atas dapat diterjemahkan ke dalam model matematika dengan sistem persamaan linear. Contoh:

- **Masalah Kecepatan Pesawat**
  - Misalkan:
    - \( v_P \) = kecepatan pesawat
    - \( v_A \) = kecepatan angin
  - Dari formula "jarak = kecepatan × waktu":
    \[
    (v_P + v_A) × 2.5 = 1500
    \]
    \[
    (v_P - v_A) × 3 = 1500
    \]
  - Disederhanakan:
    \[
    v_P + v_A = 600
    \]
    \[
    v_P - v_A = 500
    \]
  - Dengan eliminasi:
    \[
    2v_P = 1100 \Rightarrow v_P = 550
    \]
    \[
    v_A = 50
    \]
  - Hasil: Kecepatan pesawat = **550 km/jam**, kecepatan angin = **50 km/jam**.

## **4. Metode Penyelesaian SPL**
Terdapat beberapa metode penyelesaian SPL:
- **Metode Substitusi**
- **Metode Eliminasi**
- **Metode Matriks (Invers & Determinan)**
- **Metode Numerik (Jacobi & Gauss-Seidel)**

Untuk sistem dengan lebih banyak variabel dan persamaan, metode numerik lebih efektif karena kompleksitas perhitungan manual yang tinggi.

## **5. Implementasi dalam Python**
Berikut contoh penyelesaian SPL menggunakan **NumPy**:

```python
import numpy as np

# Matriks koefisien
A = np.array([[3, 2], [2, 2]])
# Vektor hasil
B = np.array([22, 16])

# Menyelesaikan sistem persamaan
X = np.linalg.solve(A, B)
print("Solusi: Buku tulis =", X[0], ", Pulpen =", X[1])
```

Kode ini menyelesaikan SPL dengan **numpy.linalg.solve()**, metode yang lebih sistematis dibanding substitusi atau eliminasi manual.