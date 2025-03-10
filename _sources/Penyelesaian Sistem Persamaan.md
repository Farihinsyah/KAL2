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
<iframe src="https://www.geogebra.org/calculator/pnqnqstt" width="800" height="600" style="border:0;"></iframe>

Misalkan sistem persamaan:

\begin{aligned}
x + 2y + 3z = 6 \\
2x + 5y + 2z = 4 \\
6x - 3y + z = 2
\end{aligned}


Langkah 1: Tulis dalam bentuk matriks augmented

\begin{bmatrix}
1 & 2 & 3 & \vert & 6 \\
2 & 5 & 2 & \vert & 4 \\
6 & -3 & 1 & \vert & 2
\end{bmatrix}


Langkah 2: Eliminasi x pada baris 2 dan baris 3 (eliminasi kolom 1)

Baris 2 = Baris 2 - 2 × Baris 1

Baris 3 = Baris 3 - 6 × Baris 1

Matriks menjadi:

\begin{bmatrix}
1 & 2 & 3 & \vert & 6 \\
0 & 1 & -4 & \vert & -8 \\
0 & -15 & -17 & \vert & -34
\end{bmatrix}


Langkah 3: Eliminasi y pada baris 3 (eliminasi kolom 2)

Baris 3 = Baris 3 + 15 × Baris 2

Matriks menjadi:

\begin{bmatrix}
1 & 2 & 3 & \vert & 6 \\
0 & 1 & -4 & \vert & -8 \\
6 & 0 & -77 & \vert & -154
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
<iframe src="https://www.geogebra.org/3d/bvhb9bbj" width="800" height="600" style="border:0;"></iframe>

Misalkan sistem persamaan:
\begin{aligned}
x + 2y + 3z = 6 \\
2x + 4y + 6z = 12 \\
3x + 6y + 9z = 18
\end{aligned}

Langkah 1: Tulis dalam bentuk matriks augmented

\begin{bmatrix}
1 & 2 & 3 & \vert & 6 \\
2 & 4 & 6 & \vert & 12 \\
3 & 6 & 9 & \vert & 18
\end{bmatrix}


Langkah 2: Eliminasi baris-baris di bawah baris 1

Baris 2 = Baris 2 - 2 × Baris 1

Matriks menjadi:

\begin{bmatrix}
1 & 2 & 3 & \vert & 6 \\
0 & 0 & 0 & \vert & 0 \\
0 & 0 & 0 & \vert & 0
\end{bmatrix}


Penyelesaian

x = 6 - 2y - 3z

Solusi umum:

x = 6 - 2y - 3z

y = y

z = z

Sistem memiliki tak hingga solusi bergantung pada y dan z
## 3. Contoh Sistem dengan Tidak Ada Solusi
<iframe src="https://www.geogebra.org/calculator/qvvtwash" width="800" height="600" style="border:0;"></iframe>

Misalkan sistem persamaan:
\begin{aligned}
x + 2y + 3z = 6 \\
2x + 4y + 6z = 12 \\
3x + 6y + 9z = 20
\end{aligned}

Langkah 1: Tulis dalam bentuk matriks augmented

\begin{bmatrix}
1 & 2 & 3 & \vert & 6 \\
2 & 4 & 6 & \vert & 12 \\
3 & 6 & 9 & \vert & 20
\end{bmatrix}


Langkah 2: Eliminasi x pada baris 2 dan baris 3

Baris 2 = Baris 2 - 2 × Baris 1

Matriks menjadi:

\begin{bmatrix}
1 & 2 & 3 & \vert & 6 \\
0 & 0 & 0 & \vert & 0 \\
0 & 0 & 0 & \vert & 2
\end{bmatrix}


Baris terakhir:

0 = 2

Sistem persamaan tidak memiliki solusi (tidak konsisten).
