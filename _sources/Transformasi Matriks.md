---
title: Transformasi Matriks

---

# Bab 5 Transformasi Matriks

* **Pengertian Transformasi Matriks**
Transformasi matriks adalah fungsi yang mengubah satu vektor menjadi vektor lain melalui perkalian matriks
Jika diberikan matriks  berukuran , kita bisa mendefinisikan sebuah fungsi  yang:
Menerima vektor kolom $\vec{x}$,
Menghasilkan vektor kolom $\vec{y}$,
Dengan aturan:
$\vec{y} = T(\vec{x}) = A \vec{x}$
Fungsi ini disebut transformasi matriks, dan termasuk dalam kelas yang lebih umum yaitu transformasi linier.

* **Visualisasi Perkalian Matriks-Vektor**
Representasi grafis dari vektor membantu memvisualisasikan bagaimana transformasi matriks bekerja. Terutama penting dalam dimensi rendah (2D/3D). Visualisasi ini banyak dipakai dalam grafik komputer.

* **Perkalian Vektor dengan Matriks**

Misalkan $A$ adalah suatu matriks, dan $\vec{x}, \vec{y}$, dan $A\vec{z}$ menjadi vektor seperti yang diberikan di bawah ini.

$A = \begin{bmatrix}
1&4 \\
2&3
\end{bmatrix}$, $\vec{x} = \begin{bmatrix}
1 \\
1
\end{bmatrix}$, $\vec{y} = \begin{bmatrix}
-1 \\
1
\end{bmatrix}$, $\vec{z} = \begin{bmatrix}
3 \\
-1
\end{bmatrix}$

Grafik $\vec{x},\vec{y}$ dan $\vec{z}$ seperti $A\vec{x}, A\vec{y}$ dan $A\vec{z}$

Dihitung:

$A\vec{x} = \begin{bmatrix}
5 \\
5
\end{bmatrix}$, $A\vec{y} = \begin{bmatrix}
3 \\
1
\end{bmatrix}$, dan $A\vec{z} = \begin{bmatrix}
-1 \\
3
\end{bmatrix}$

* **Menggabungkan Penjumlahan dan Perkalian Matriks**

Misalkan $A$ adalah suatu matriks, dan $\vec{x}$ dan $\vec{y}$ menjadi vektor seperti yang diberikan di bawah ini.

$A = \begin{bmatrix}
1&1 \\
1&2
\end{bmatrix}$, $\vec{x} = \begin{bmatrix}
2 \\
1
\end{bmatrix}$, $\vec{y} = \begin{bmatrix}
-1 \\
1
\end{bmatrix}$

Sketsa $\vec{x}+\vec{y},A\vec{x},A\vec{y}$ dan $A(\vec{x}+\vec{y})$

Dihitung:

$\vec{x}+\vec{y}= \begin{bmatrix}
1 \\
2
\end{bmatrix}$; $A\vec{x} = \begin{bmatrix}
3 \\
4
\end{bmatrix}$; $A\vec{y} = \begin{bmatrix}
0 \\
1
\end{bmatrix}$, $A(\vec{x}+\vec{y}) = \begin{bmatrix}
3 \\
5
\end{bmatrix}$

Ini menunjukkan sifat distributif dari perkalian matriks terhadap penjumlahan vektor.

$A(\vec{x}+\vec{y})=A\vec{x}+A\vec{y}$

* **Membuat Sketsa Efek Perkalian Matriks**

Diberikan $A, \vec{x}, \vec{y}$ dan $\vec{z}$ seperti yang diberikan di bawah ini.

$A = \begin{bmatrix}
1&-1 \\
1&-1
\end{bmatrix}$, $\vec{x} = \begin{bmatrix}
1 \\
1
\end{bmatrix}$, $\vec{y} = \begin{bmatrix}
-1 \\
1
\end{bmatrix}$, $\vec{z} = \begin{bmatrix}
4 \\
1
\end{bmatrix}$

Grafik $\vec{x},\vec{y}$ dan $\vec{z}$ seperti $A\vec{x}, A\vec{y}$ dan $A\vec{z}$

Dihitung:

$A\vec{x} = \begin{bmatrix}
0 \\
0
\end{bmatrix}$, $A\vec{y} = \begin{bmatrix}
-2 \\
-2
\end{bmatrix}$, dan $A\vec{z} = \begin{bmatrix}
3 \\
3
\end{bmatrix}$

* **Jenis-Jenis Transformasi Matriks**
1. Horizontal Stretch $\begin{bmatrix}
k&0 \\
0&1
\end{bmatrix}$
2. Vertical Stretch $\begin{bmatrix}
1&0 \\
0&k
\end{bmatrix}$
3. Horizontal Shear $\begin{bmatrix}
1&k \\
0&1
\end{bmatrix}$
4. Vertical Shear $\begin{bmatrix}
1&0 \\
k&1
\end{bmatrix}$
5. Horizontal Reflection $\begin{bmatrix}
-1&0 \\
0&1
\end{bmatrix}$
6. Vertical Reflection $\begin{bmatrix}
1&0 \\
0&-1
\end{bmatrix}$
7. Diagonal Reflection $\begin{bmatrix}
0&1 \\
1&0
\end{bmatrix}$
8. Rotation $\begin{bmatrix}
\cos\theta&-\sin\theta \\
\sin\theta&\cos\theta
\end{bmatrix}$
9. Projection $\begin{bmatrix}
1&0 \\
0&0
\end{bmatrix}$



### Mengerjakan Halaman 239

**Nomor 1**

Diberikan matriks $A$. Sketsa $\vec{x}, \vec{y}, A\vec{x}$ dan $A\vec{y}$ pada sumbu kartesian yang sama, dimana $\vec{x} = \begin{bmatrix}
1 \\
1
\end{bmatrix}$ dan $\vec{y} = \begin{bmatrix}
-1 \\
2
\end{bmatrix}$

Soal : $A = \begin{bmatrix}
1 & -1 \\
2 & 3
\end{bmatrix}$

Diketahui:
$\vec{x} = \begin{bmatrix}
1 \\
1
\end{bmatrix}$, $\vec{y} = \begin{bmatrix}
-1 \\
2
\end{bmatrix}$, $A = \begin{bmatrix}
1 & -1 \\
2 & 3
\end{bmatrix}$

Langkah-langkah:
1. Kalikan $A$ dengan $\vec{x}$:
$A\vec{x} =
\begin{bmatrix}
1 & -1 \\
2 & 3
\end{bmatrix}
\begin{bmatrix}
1 \\
1
\end{bmatrix} =
\begin{bmatrix}
1 & -1 \\
2 & +3
\end{bmatrix} =
\begin{bmatrix}
0 \\
5
\end{bmatrix}$

2. Kalikan $A$ dengan $\vec{y}$:
$A\vec{y} =
\begin{bmatrix}
1 & -1 \\
2 & 3
\end{bmatrix}
\begin{bmatrix}
-1 \\
2
\end{bmatrix} =
\begin{bmatrix}
-1 & -2 \\
-2 & +6
\end{bmatrix} =
\begin{bmatrix}
-3 \\
4
\end{bmatrix}$

Hasil:
$\vec{x} = (1,1)$
$\vec{y} = (-1,2)$
$A\vec{x} = (0,5)$
$A\vec{y} = (-3,4)$

**Nomor 2**

Diberikan matriks $A$. Sketsa $\vec{x}, \vec{y}, A\vec{x}$ dan $A\vec{y}$ pada sumbu kartesian yang sama, dimana $\vec{x} = \begin{bmatrix}
1 \\
1
\end{bmatrix}$ dan $\vec{y} = \begin{bmatrix}
-1 \\
2
\end{bmatrix}$

Soal : $A = \begin{bmatrix}
2 & 0 \\
-1 & 3
\end{bmatrix}$

Diketahui:
$\vec{x} = \begin{bmatrix}
1 \\
1
\end{bmatrix}$, $\vec{y} = \begin{bmatrix}
-1 \\
2
\end{bmatrix}$, $A = \begin{bmatrix}
2 & 0 \\
-1 & 3
\end{bmatrix}$

Langkah-langkah:
1. Kalikan $A$ dengan $\vec{x}$:
$A\vec{x} =
\begin{bmatrix}
2 & 0 \\
-1 & 3
\end{bmatrix}
\begin{bmatrix}
1 \\
1
\end{bmatrix} =
\begin{bmatrix}
2 & 0 \\
-1 & +3
\end{bmatrix} =
\begin{bmatrix}
2 \\
2
\end{bmatrix}$

2. Kalikan $A$ dengan $\vec{y}$:
$A\vec{y} =
\begin{bmatrix}
2 & 0 \\
-1 & 3
\end{bmatrix}
\begin{bmatrix}
-1 \\
2
\end{bmatrix} =
\begin{bmatrix}
-2 & 0 \\
1 & +6
\end{bmatrix} =
\begin{bmatrix}
-2 \\
7
\end{bmatrix}$

**Nomor 5**

Sketsa persegi satuan yang telah ditransformasikan diberikan. Temukan matriks $A$ yang melakukan transformasi ini 

![IMG_20250413_222525](https://hackmd.io/_uploads/Sy8z_8tRyl.jpg)


Dari gambar:
- Titik (1,0) dipetakan ke (1,2)
- Titik (0,1) dipetakan ke (1,3)

Berarti:
$A
\begin{bmatrix}
1 \\
0
\end{bmatrix} =
\begin{bmatrix}
1 \\
2
\end{bmatrix},
A
\begin{bmatrix}
0 \\
1
\end{bmatrix} =
\begin{bmatrix}
1 \\
3
\end{bmatrix}$

Sehingga matriks $A$ memiliki kolol-kolom:
$A =
\begin{bmatrix}
1 & 1 \\
2 & 3
\end{bmatrix}$

**Nomor 6**

Sketsa persegi satuan yang telah ditransformasikan diberikan. Temukan matriks $A$ yang melakukan transformasi ini

![IMG_20250413_222549](https://hackmd.io/_uploads/ry4U_UKCkl.jpg)


Dari gambar:
- Titik (1,0) dipetakan ke (1,1)
- Titik (0,1) dipetakan ke (-1,1)

Berarti:
$A
\begin{bmatrix}
1 \\
0
\end{bmatrix} =
\begin{bmatrix}
1 \\
1
\end{bmatrix},
A
\begin{bmatrix}
0 \\
1
\end{bmatrix} =
\begin{bmatrix}
-1 \\
1
\end{bmatrix}$

Sehingga matriks $A$ memiliki kolol-kolom:
$A =
\begin{bmatrix}
1 & -1 \\
1 & 1
\end{bmatrix}$