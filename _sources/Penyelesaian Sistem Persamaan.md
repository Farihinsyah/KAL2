---
title: 'Penyelesaian Sistem Persamaan '

---

## Penyelesaian Sistem Persamaan Linier 3 Variabel dengan Eliminasi Gauss
Sebuah sistem persamaan linier dengan 3 variabel bisa memiliki:
1. **Satu Solusi** = Sistem memiliki solusi unik dan determinan matriks koefisien tidak sama dengan nol.
2. **Banyak Solusi** = Sistem memiliki solusi, tetapi ada variabel yang nilainya bebas atau tidak terikat.
3. **Tidak Ada Solusi** = Sistem tidak memiliki solusi karena terjadi pertentangan antar persamaan.
---
## 1. Contoh Sistem dengan Satu Solusi
https://www.geogebra.org/calculator/pnqnqstt
Misalkan sistem persamaan:
\
\begin{cases}
x + 2y + 3z = 6 \\
2x + 5y + 2z = 4 \\
6x - 3y + z = 2
\end{cases}
Langkah 1: Tulis dalam bentuk matriks augmented

\begin{bmatrix}
1 & 2 & 3 & | & 6 \\
2 & 5 & 2 & | & 4 \\
6 & -3 & 1 & | & 2
\end{bmatrix}

Langkah 2: Eliminasi x pada baris 2 dan baris 3 (eliminasi kolom 1)

Baris 2 = Baris 2 - 2 × Baris 1

Baris 3 = Baris 3 - 6 × Baris 1

Matriks menjadi:

\begin{bmatrix}
1 & 2 & 3 & | & 6 \\
0 & 1 & -4 & | & -8 \\
0 & -15 & -17 & | & -34
\end{bmatrix}

Langkah 3: Eliminasi y pada baris 3 (eliminasi kolom 2)

Baris 3 = Baris 3 + 15 × Baris 2

Matriks menjadi:

\begin{bmatrix}
1 & 2 & 3 & | & 6 \\
0 & 1 & -4 & | & -8 \\
0 & 0 & -77 & | & -154
\end{bmatrix}

Langkah 4: Substitusi Balik

Dari baris 3:


-77z = -154
z = 2

y - 4(2) = -8
y - 8 = -8
y = 0

x + 2(0) + 3(2) = 6
x = 0

Hasil Akhir

(x, y, z) = (0, 0, 2)
## 2. Contoh Sistem dengan Banyak Solusi
https://www.geogebra.org/3d/bvhb9bbj
Misalkan sistem persamaan:
\begin{cases}
x + 2y + 3z = 6 \\
2x + 4y + 6z = 12 \\
3x + 6y + 9z = 18
\end{cases}

Langkah 1: Tulis dalam bentuk matriks augmented

\begin{bmatrix}
1 & 2 & 3 & | & 6 \\
2 & 4 & 6 & | & 12 \\
3 & 6 & 9 & | & 18
\end{bmatrix}

Langkah 2: Eliminasi baris-baris di bawah baris 1

Baris 2 = Baris 2 - 2 × Baris 1

Matriks menjadi:

\begin{bmatrix}
1 & 2 & 3 & | & 6 \\
0 & 0 & 0 & | & 0 \\
0 & 0 & 0 & | & 0
\end{bmatrix}

Penyelesaian

x = 6 - 2y - 3z

Solusi umum:

x = 6 - 2y - 3z

y = y

z = z

Sistem memiliki tak hingga solusi bergantung pada y dan z
## 3. Contoh Sistem dengan Tidak Ada Solusi
https://www.geogebra.org/calculator/qvvtwash
Misalkan sistem persamaan:
\begin{cases}
x + 2y + 3z = 6 \\
2x + 4y + 6z = 12 \\
3x + 6y + 9z = 20
\end{cases}Langkah 1: Tulis dalam bentuk matriks augmented

\begin{bmatrix}
1 & 2 & 3 & | & 6 \\
2 & 4 & 6 & | & 12 \\
3 & 6 & 9 & | & 20
\end{bmatrix}

Langkah 2: Eliminasi x pada baris 2 dan baris 3

Baris 2 = Baris 2 - 2 × Baris 1

Matriks menjadi:

\begin{bmatrix}
1 & 2 & 3 & | & 6 \\
0 & 0 & 0 & | & 0 \\
0 & 0 & 0 & | & 2
\end{bmatrix}

Analisis

Baris terakhir:

0 = 2

Sistem persamaan tidak memiliki solusi (tidak konsisten).
