---
title: Transformasi Matriks

---

# Transformasi Matriks

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

* **Menvisualisasikan Transformasi Matriks Menggunakan Vektor***

Gambarkan vektor persegi satuan sebelum dan sesudah dikalikan dengan $A$. Di mana

$A = \begin{bmatrix}
1&4 \\
2&3
\end{bmatrix}$

Solusi. Keempat sudut persegi satuan dapat direpresentasikan dengan vektor

$\begin{bmatrix}
0 \\
0
\end{bmatrix}$, $\begin{bmatrix}
1 \\
0
\end{bmatrix}$, $\begin{bmatrix}
1 \\
1
\end{bmatrix}$, $\begin{bmatrix}
0 \\
1
\end{bmatrix}$

Mengalikan masing-masing dengan $A$ menghasilkan vektor

$\begin{bmatrix}
0 \\
0
\end{bmatrix}$, $\begin{bmatrix}
1 \\
2
\end{bmatrix}$, $\begin{bmatrix}
5 \\
5
\end{bmatrix}$, $\begin{bmatrix}
4 \\
3
\end{bmatrix}$

masing-masing.
(Petunjuk : salah satu cara menggunakan kalkulator untuk melakukan ini dengan cepat adalah membuat matriks 2 x 4 yang kolomnya masing-masing adalah vektor ini. Dalam hal ini. buat matriks

$B = \begin{bmatrix}
0&1&1&0 \\
0&0&1&1
\end{bmatrix}$

Kemudian kalikan $B$ dengan $A$ dan baca vektor yang ditansformasikan dari kolom masing-masing:

$AB = \begin{bmatrix}
0&1&5&4 \\
0&2&5&3
\end{bmatrix}$

Ini menghemat waktu, terutama jika Anda melakukan prosedur serupa untuk beberapa matriks $A$. Tentu saja kita dapat menghemat lebih banyak waktu dengan melewatkan kolom pertama; karena ini adalah kolom nol)

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

Hasil:
$\vec{x} = (1,1)$
$\vec{y} = (-1,2)$
$A\vec{x} = (2,2)$
$A\vec{y} = (-2,7)$

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



---
---



## Pembuktian Transformasi Linier

Diberikan transformasi:

$$
T(v_1, v_2) = (v_1 + v_2,\ v_1)
$$

Kita ingin membuktikan bahwa $T$ adalah *transformasi linier*, yaitu memenuhi dua sifat:

1. *Additivitas*:  
   $T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})$

2. *Homogenitas (Perkalian skalar)*:  
   $T(c\mathbf{u}) = cT(\mathbf{u})$

---

### 1. Pembuktian Additivitas

Misalkan dua vektor di $\mathbb{R}^2$:

$$
\mathbf{u} = (u_1, u_2), \quad \mathbf{v} = (v_1, v_2)
$$

#### Langkah 1: Hitung penjumlahan vektor
$$
\mathbf{u} + \mathbf{v} = (u_1 + v_1,\ u_2 + v_2)
$$

#### Langkah 2: Hitung sisi kiri dari sifat additivitas

$$
T(\mathbf{u} + \mathbf{v}) = T(u_1 + v_1,\ u_2 + v_2)
$$

Definisi $T$ mengatakan bahwa komponen pertama adalah penjumlahan dari dua komponen vektor input, dan komponen kedua adalah komponen pertama dari input itu sendiri. Maka:

\begin{align*}
T(\mathbf{u} + \mathbf{v}) 
&= ((u_1 + v_1) + (u_2 + v_2),\ u_1 + v_1) \\
&= (u_1 + u_2 + v_1 + v_2,\ u_1 + v_1)
\end{align*}

#### Langkah 3: Hitung sisi kanan

Pertama, kita hitung:

\begin{align*}
T(\mathbf{u}) &= (u_1 + u_2,\ u_1) \\
T(\mathbf{v}) &= (v_1 + v_2,\ v_1)
\end{align*}

Kemudian jumlahkan kedua hasilnya:

\begin{align*}
T(\mathbf{u}) + T(\mathbf{v}) 
&= (u_1 + u_2 + v_1 + v_2,\ u_1 + v_1)
\end{align*}

#### Kesimpulan Additivitas:

Karena:

$$
T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})
$$

maka *sifat additivitas terpenuhi*.

---

### 2. Pembuktian Homogenitas

Misalkan $\mathbf{u} = (u_1, u_2)$ dan $c$ adalah sembarang skalar di $\mathbb{R}$.

#### Langkah 1: Hitung perkalian skalar

$$
c \cdot \mathbf{u} = (cu_1,\ cu_2)
$$

#### Langkah 2: Hitung sisi kiri

$$
T(c\mathbf{u}) = T(cu_1,\ cu_2)
$$

Menggunakan definisi $T$:

\begin{align*}
T(c\mathbf{u}) 
&= (cu_1 + cu_2,\ cu_1) \\
&= c(u_1 + u_2,\ u_1)
\end{align*}

#### Langkah 3: Hitung sisi kanan

\begin{align*}
T(\mathbf{u}) &= (u_1 + u_2,\ u_1) \\
c \cdot T(\mathbf{u}) &= c(u_1 + u_2,\ u_1) = (cu_1 + cu_2,\ cu_1)
\end{align*}

#### Kesimpulan Homogenitas:

Karena:

$$
T(c\mathbf{u}) = cT(\mathbf{u})
$$

maka *sifat homogenitas terpenuhi*.

---

### Kesimpulan Akhir:

Karena transformasi $T$ memenuhi:

- *Additivitas*: $T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})$
- *Homogenitas*: $T(c\mathbf{u}) = cT(\mathbf{u})$

maka:

$$
\boxed{T(v_1, v_2) = (v_1 + v_2,\ v_1) \text{ adalah transformasi linier}}
$$



---


---



## Contoh Transformasi Refleksi (Dengan Matriks dan Titik)

Berikut adalah contoh 2 titik untuk masing-masing jenis refleksi:

---

### 1. Refleksi terhadap sumbu-$x$

Matriks transformasi:

$$
\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}
$$

Contoh titik:

- $A(2, 3) \rightarrow A'(2, -3)$  
- $B(-1, -4) \rightarrow B'(-1, 4)$
<iframe src="https://www.geogebra.org/calculator/csfvpra4" width="600" height="400" style="border:0;"></iframe>


---

### 2. Refleksi terhadap sumbu-$y$

Matriks transformasi:

$$
\begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}
$$

Contoh titik:

- $A(3, 2) \rightarrow A'(-3, 2)$  
- $B(-2, -1) \rightarrow B'(2, -1)$
<iframe src="https://www.geogebra.org/calculator/fsn5nrva" width="600" height="400" style="border:0;"></iframe>

---

### 3. Refleksi terhadap garis $y = x$

Matriks transformasi:

$$
\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}
$$

Contoh titik:

- $A(1, 4) \rightarrow A'(4, 1)$  
- $B(-3, 2) \rightarrow B'(2, -3)$
<iframe src="https://www.geogebra.org/calculator/qrbyjpfu" width="600" height="400" style="border:0;"></iframe>

---

### 4. Refleksi terhadap garis $y = -x$

Matriks transformasi:

$$
\begin{bmatrix} 0 & -1 \\ -1 & 0 \end{bmatrix}
$$

Contoh titik:

- $A(2, 5) \rightarrow A'(-5, -2)$  
- $B(-1, -4) \rightarrow B'(4, 1)$
<iframe src="https://www.geogebra.org/calculator/s7cmjmew" width="600" height="400" style="border:0;"></iframe>

---

### 5. Refleksi terhadap titik asal (origin)

Matriks transformasi:

$$
\begin{bmatrix} -1 & 0 \\ 0 & -1 \end{bmatrix}
$$

Contoh titik:

- $A(3, -2) \rightarrow A'(-3, 2)$  
- $B(-5, 1) \rightarrow B'(5, -1)$
<iframe src="https://www.geogebra.org/calculator/qyg5yjf9" width="600" height="400" style="border:0;"></iframe>



---
---



## Penjelasan Refleksi Titik terhadap Garis \( y = 2 \)

Dalam transformasi geometri, refleksi titik terhadap suatu garis dapat dilakukan menggunakan matriks dan translasi. Pada kasus ini, kita akan merefleksikan titik terhadap garis horizontal \( y = 2 \). Berikut adalah penjelasan langkah-langkah yang diambil dalam proses refleksi tersebut.

### Langkah 1: Matriks Refleksi terhadap Sumbu-X

Untuk refleksi terhadap garis horizontal \( y = 2 \), kita perlu menggunakan dua operasi dasar:

1. **Refleksi terhadap sumbu-X:** 
   Matriks refleksi terhadap sumbu-X membalikkan koordinat \( y \) dari titik yang diberikan. Matriks refleksi terhadap sumbu-X adalah:

   $$
   B = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}
   $$

   Matriks ini membalikkan koordinat \( y \), tetapi tidak mengubah \( x \).

### Langkah 2: Translasi untuk Menyesuaikan dengan Garis \( y = 2 \)

Setelah refleksi terhadap sumbu-X, kita perlu melakukan **translasi** agar titik hasil refleksi berada pada posisi yang benar relatif terhadap garis \( y = 2 \). Garis \( y = 2 \) berada pada jarak 2 satuan di atas sumbu-X. Oleh karena itu, kita perlu menambahkan vektor translasi yang menggeser hasil refleksi ke posisi yang tepat.

Vektor translasi yang digunakan adalah:

$$
t = \begin{bmatrix} 0 \\ 4 \end{bmatrix}
$$

Vektor ini menggeser titik hasil refleksi sebesar 4 satuan di atas sumbu-X untuk mencapai garis \( y = 2 \).

### Langkah 3: Menghitung Titik Refleksi

Titik asal yang akan direfleksikan adalah \( (x, y) = (1, 1) \). Proses refleksi dilakukan dengan matriks transformasi yang terdiri dari refleksi dan translasi:

$$
B_{\text{trans}} = B \cdot \begin{bmatrix} x \\ y \end{bmatrix} + t
$$

Substitusi koordinat \( (x, y) = (1, 1) \) ke dalam persamaan ini menghasilkan:

$$
B_{\text{trans}} = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 1 \end{bmatrix} + \begin{bmatrix} 0 \\ 4 \end{bmatrix} = \begin{bmatrix} 1 \\ -1 \end{bmatrix} + \begin{bmatrix} 0 \\ 4 \end{bmatrix} = \begin{bmatrix} 1 \\ 3 \end{bmatrix}
$$

Dengan demikian, titik hasil refleksi adalah \( (1, 3) \).

### Langkah 4: Visualisasi Grafik

Untuk memvisualisasikan refleksi ini, kita menggambar titik asal dan titik hasil refleksi pada grafik. Titik asal diberi tanda merah (ro), dan titik hasil refleksi diberi tanda biru (bo). Garis \( y = 2 \) juga digambarkan sebagai garis hijau.

#### Grafik:

1. **Titik asal:** Titik \( (1, 1) \) digambarkan dengan tanda merah.
2. **Titik hasil refleksi:** Titik \( (1, 3) \) digambarkan dengan tanda biru.
3. **Garis \( y = 2 \):** Garis hitam sebagai garis refleksi.
4. **Garis horizontal:** Untuk menunjukkan sumbu X dan Y yang digunakan sebagai referensi.

```python
koordinats = np.array([[1], [1]])
x = koordinats[0,:]
y = koordinats[1,:]

B = np.array([[1,0],[0,-1]])
t = np.array([[0],[4]])
B_trans = B @ koordinats + t

x_LT2 = B_trans[0,:]
y_LT2 = B_trans[1,:]

fig, ax = plt.subplots()

# Titik asal (merah)
ax.plot(x, y, 'ro', label="Asal (Domain)")

# Titik bayangan (biru)
ax.plot(x_LT2, y_LT2, 'bo', label="Bayangan (Codomain)")

# Garis putus-putus antara asal
ax.plot(x, y, 'r', ls="--")

# Garis refleksi biru
ax.plot(x_LT2, y_LT2, 'b')

# Garis refleksi y = 2
ax.axhline(y=2, color="black", ls="--", label="y = 2")

# Sumbu koordinat
ax.axvline(x=0, color="k", ls=":")
ax.axhline(y=0, color="k", ls=":")

ax.grid(True)
ax.axis([0,4,0,4])
ax.set_aspect('equal')
ax.set_title("Refleksi terhadap Sumbu Y = 2")

# Menampilkan legenda
ax.legend()
```

![alt text](image.png)


---

## Penjelasan Refleksi Titik terhadap Garis \( x = 2 \)

Dalam transformasi geometri, refleksi titik terhadap suatu garis dapat dilakukan dengan menggunakan matriks refleksi dan translasi. Pada kasus ini, kita akan merefleksikan titik terhadap garis vertikal \( x = 2 \). Berikut adalah penjelasan langkah-langkah yang diambil dalam proses refleksi tersebut.

### Langkah 1: Matriks Refleksi terhadap Sumbu-Y

Untuk refleksi terhadap garis vertikal \( x = 2 \), kita perlu menggunakan dua operasi dasar:

1. **Refleksi terhadap sumbu-Y:**
   Matriks refleksi terhadap sumbu-Y membalikkan koordinat \( x \) dari titik yang diberikan. Matriks refleksi terhadap sumbu-Y adalah:

   $$
   B = \begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}
   $$

   Matriks ini membalikkan koordinat \( x \), tetapi tidak mengubah \( y \).

### Langkah 2: Translasi untuk Menyesuaikan dengan Garis \( x = 2 \)

Setelah refleksi terhadap sumbu-Y, kita perlu melakukan **translasi** agar titik hasil refleksi berada pada posisi yang benar relatif terhadap garis \( x = 2 \). Garis \( x = 2 \) berada pada jarak 2 satuan di sebelah kanan sumbu-Y. Oleh karena itu, kita perlu menambahkan vektor translasi yang menggeser hasil refleksi ke posisi yang tepat.

Vektor translasi yang digunakan adalah:

$$
t = \begin{bmatrix} 4 \\ 0 \end{bmatrix}
$$

Vektor ini menggeser titik hasil refleksi sebesar 4 satuan ke kanan sumbu-Y untuk mencapai garis \( x = 2 \).

### Langkah 3: Menghitung Titik Refleksi

Titik asal yang akan direfleksikan adalah \( (x, y) = (1, 1) \). Proses refleksi dilakukan dengan matriks transformasi yang terdiri dari refleksi dan translasi:

$$
B_{\text{trans}} = B \cdot \begin{bmatrix} x \\ y \end{bmatrix} + t
$$

Substitusi koordinat \( (x, y) = (1, 1) \) ke dalam persamaan ini menghasilkan:

$$
B_{\text{trans}} = \begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 1 \end{bmatrix} + \begin{bmatrix} 4 \\ 0 \end{bmatrix} = \begin{bmatrix} -1 \\ 1 \end{bmatrix} + \begin{bmatrix} 4 \\ 0 \end{bmatrix} = \begin{bmatrix} 3 \\ 1 \end{bmatrix}
$$

Dengan demikian, titik hasil refleksi adalah \( (3, 1) \).

### Langkah 4: Visualisasi Grafik

Untuk memvisualisasikan refleksi ini, kita menggambar titik asal dan titik hasil refleksi pada grafik. Titik asal diberi tanda merah (ro), dan titik hasil refleksi diberi tanda biru (bo). Garis \( x = 2 \) juga digambarkan sebagai garis hitam.

#### Grafik:

1. **Titik asal:** Titik \( (1, 1) \) digambarkan dengan tanda merah.
2. **Titik hasil refleksi:** Titik \( (3, 1) \) digambarkan dengan tanda biru.
3. **Garis \( x = 2 \):** Garis hitam sebagai garis refleksi.
4. **Garis sumbu X dan Y:** Untuk menunjukkan sumbu referensi.

```python
koordinats = np.array([[1], [1]])
x = koordinats[0,:]
y = koordinats[1,:]

B = np.array([[-1,0],[0,1]])
t = np.array([[4],[0]])
B_trans = B @ koordinats + t

x_LT2 = B_trans[0,:]
y_LT2 = B_trans[1,:]

fig, ax = plt.subplots()

# Titik asal (merah)
ax.plot(x, y, 'ro', label="Asal (Domain)")

# Titik bayangan (biru)
ax.plot(x_LT2, y_LT2, 'bo', label="Bayangan (Codomain)")

# Garis putus-putus antara asal
ax.plot(x, y, 'r', ls="--")

# Garis refleksi biru
ax.plot(x_LT2, y_LT2, 'b')

# Garis refleksi x = 2 (hitam putus-putus)
ax.axvline(x=2, color="black", ls="--", label="x = 2")

# Sumbu koordinat
ax.axvline(x=0, color="k", ls=":")
ax.axhline(y=0, color="k", ls=":")

ax.grid(True)
ax.axis([0,4,0,4])
ax.set_aspect('equal')
ax.set_title("Refleksi terhadap Sumbu X = 2")

# Menampilkan legenda
ax.legend()
```


![alt text](image-1.png)


---

## Penjelasan Refleksi Titik terhadap Garis \( y = x \)

Refleksi titik terhadap garis \( y = x \) adalah transformasi geometri di mana titik asal dipindahkan sehingga posisinya simetris terhadap garis tersebut. Untuk memahami proses ini, mari kita lihat langkah-langkah berikut.

### Langkah 1: Matriks Refleksi terhadap Garis \( y = x \)

Refleksi terhadap garis \( y = x \) dapat dilakukan dengan menggunakan matriks transformasi. Matriks refleksi untuk garis \( y = x \) dapat dinyatakan sebagai:

$$
B = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}
$$

Matriks ini bertukar posisi komponen \( x \) dan \( y \) dari titik yang diberikan. Jadi, setelah diterapkan, koordinat titik \( (x, y) \) akan menjadi \( (y, x) \).

### Langkah 2: Menghitung Titik Refleksi

Titik asal yang akan direfleksikan adalah \( (x, y) = (1, 2) \). Proses refleksi dilakukan dengan mengalikan matriks refleksi \( B \) dengan vektor koordinat asal \( (x, y) \):

$$
B_{\text{trans}} = B \cdot \begin{bmatrix} x \\ y \end{bmatrix}
$$

Substitusi koordinat \( (x, y) = (1, 2) \) ke dalam persamaan ini menghasilkan:

$$
B_{\text{trans}} = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 2 \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
$$

Dengan demikian, titik hasil refleksi adalah \( (2, 1) \).

### Langkah 3: Visualisasi Grafik

Untuk memvisualisasikan refleksi ini, kita menggambar titik asal dan titik hasil refleksi pada grafik. Titik asal diberi tanda merah (ro), dan titik hasil refleksi diberi tanda biru (bo). Garis \( y = x \) digambarkan sebagai garis hitam.

#### Grafik:

1. **Titik asal:** Titik \( (1, 2) \) digambarkan dengan tanda merah.
2. **Titik hasil refleksi:** Titik \( (2, 1) \) digambarkan dengan tanda biru.
3. **Garis \( y = x \):** Garis hitam sebagai garis refleksi.
4. **Garis sumbu X dan Y:** Untuk menunjukkan sumbu referensi.

```python
koordinats = np.array([[1], [2]])
x = koordinats[0,:]
y = koordinats[1,:]

B = np.array([[0,1],[1,0]])
B_trans = B @ koordinats

x_LT2 = B_trans[0,:]
y_LT2 = B_trans[1,:]

fig, ax = plt.subplots()

# Titik asal (merah)
ax.plot(x, y, 'ro', label="Asal (Domain)")

# Titik bayangan (biru)
ax.plot(x_LT2, y_LT2, 'bo', label="Bayangan (Codomain)")

# Garis putus-putus dari titik asal
ax.plot(x, y, 'r', ls="--")

# Garis dari bayangan
ax.plot(x_LT2, y_LT2, 'b')

# Garis refleksi y = x (hitam putus-putus)
ax.plot([0, 4], [0, 4], color="black", ls="--", label="y = x")

# Sumbu koordinat
ax.axvline(x=0, color="k", ls=":")
ax.axhline(y=0, color="k", ls=":")

ax.grid(True)
ax.axis([0,4,0,4])
ax.set_aspect('equal')
ax.set_title("Refleksi terhadap garis y = x")

# Menampilkan legenda
ax.legend()

```

![alt text](image-2.png)
