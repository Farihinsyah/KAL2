---
title: Pembuktian Transformasi Linier

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
<iframe src="https://www.geogebra.org/calculator/csfvpra4" width="600" height="400" style="border:0;"></iframe>


---

### 2. Refleksi terhadap sumbu-$y$

Matriks transformasi:

$$
\begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}
$$

Contoh titik:

- $A(3, 2) \rightarrow A'(-3, 2)$  
<iframe src="https://www.geogebra.org/calculator/fsn5nrva" width="600" height="400" style="border:0;"></iframe>

---

### 3. Refleksi terhadap garis $y = x$

Matriks transformasi:

$$
\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}
$$

Contoh titik:

- $A(1, 4) \rightarrow A'(4, 1)$  
<iframe src="https://www.geogebra.org/calculator/qrbyjpfu" width="600" height="400" style="border:0;"></iframe>

---

### 4. Refleksi terhadap garis $y = -x$

Matriks transformasi:

$$
\begin{bmatrix} 0 & -1 \\ -1 & 0 \end{bmatrix}
$$

Contoh titik:

- $A(2, 5) \rightarrow A'(-5, -2)$  
<iframe src="https://www.geogebra.org/calculator/s7cmjmew" width="600" height="400" style="border:0;"></iframe>

---

### 5. Refleksi terhadap titik asal (origin)

Matriks transformasi:

$$
\begin{bmatrix} -1 & 0 \\ 0 & -1 \end{bmatrix}
$$

Contoh titik:

- $A(3, -2) \rightarrow A'(-3, 2)$  
<iframe src="https://www.geogebra.org/calculator/qyg5yjf9" width="600" height="400" style="border:0;"></iframe>
