---
title: Hasil Kali Silang (Cross Product)

---

# Hasil Kali Silang (Cross Product)

## Pengertian

Hasil kali silang adalah operasi antara dua vektor tiga dimensi yang menghasilkan **vektor baru**.

Perkalian silang dari dua vektor $\mathbf{u}$ dan $\mathbf{v}$ didefinisikan sebagai:

$$
\mathbf{u} = \begin{bmatrix} u_1 \\ u_2 \\ u_3 \end{bmatrix}, \quad
\mathbf{v} = \begin{bmatrix} v_1 \\ v_2 \\ v_3 \end{bmatrix}
$$

Maka:

$$
\mathbf{u} \times \mathbf{v} =
\begin{bmatrix}
u_2v_3 - u_3v_2 \\
u_3v_1 - u_1v_3 \\
u_1v_2 - u_2v_1
\end{bmatrix}
$$

Atau dalam bentuk determinan:

$$
\mathbf{u} \times \mathbf{v} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3
\end{vmatrix}
= (u_2v_3 - u_3v_2)\hat{i} - (u_1v_3 - u_3v_1)\hat{j} + (u_1v_2 - u_2v_1)\hat{k}
$$

---

## Sifat-sifat Perkalian Silang

1. **Sifat Antikomutatif (Anticommutative Property)**  
   $$
   \vec{u} \times \vec{v} = -(\vec{v} \times \vec{u})
   $$

2. **Sifat Distributif terhadap Penjumlahan (Distributive Properties)**  
   a. 
   $$
   (\vec{u} + \vec{v}) \times \vec{w} = \vec{u} \times \vec{w} + \vec{v} \times \vec{w}
   $$
   b. 
   $$
   \vec{u} \times (\vec{v} + \vec{w}) = \vec{u} \times \vec{v} + \vec{u} \times \vec{w}
   $$

3. **Sifat Asosiatif terhadap Perkalian Skalar**  
   $$
   c(\vec{u} \times \vec{v}) = (c\vec{u}) \times \vec{v} = \vec{u} \times (c\vec{v})
   $$

4. **Sifat Ortogonalitas (Orthogonality Properties)**  
   a. 
   $$
   (\vec{u} \times \vec{v}) \cdot \vec{u} = 0
   $$
   b. 
   $$
   (\vec{u} \times \vec{v}) \cdot \vec{v} = 0
   $$

5. **Perkalian Silang Vektor dengan Dirinya Sendiri**  
   $$
   \vec{u} \times \vec{u} = \vec{0}
   $$

6. **Perkalian Silang dengan Vektor Nol**  
   $$
   \vec{u} \times \vec{0} = \vec{0}
   $$

7. **Triple Scalar Product (Perkalian Titik dari Perkalian Silang)**  
   $$
   \vec{u} \cdot (\vec{v} \times \vec{w}) = (\vec{u} \times \vec{v}) \cdot \vec{w}
   $$


---

### Contoh 1

Misalkan:

$$
\mathbf{u} = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}, \quad
\mathbf{v} = \begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/dpdpqwyq" width="600" height="400" style="border:0;"></iframe>

$$
\mathbf{u} \times \mathbf{v} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3
\end{vmatrix}
= (u_2v_3 - u_3v_2)\hat{i} - (u_1v_3 - u_3v_1)\hat{j} + (u_1v_2 - u_2v_1)\hat{k}
$$

Hitung:

$$
\begin{bmatrix}
0 \cdot 0 - 0 \cdot 1 \\
-(1 \cdot 0 - 0 \cdot 0) \\
1 \cdot 1 - 0 \cdot 0
\end{bmatrix} =
\begin{bmatrix}
0 \\
0 \\
1
\end{bmatrix}
$$

---

### Contoh 2

Misalkan:

$$
\mathbf{u} = \begin{bmatrix} 2 \\ 3 \\ 4 \end{bmatrix}, \quad
\mathbf{v} = \begin{bmatrix} 5 \\ 6 \\ 7 \end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/s2tcbt9f" width="600" height="400" style="border:0;"></iframe>

$$
\mathbf{u} \times \mathbf{v} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3
\end{vmatrix}
= (u_2v_3 - u_3v_2)\hat{i} - (u_1v_3 - u_3v_1)\hat{j} + (u_1v_2 - u_2v_1)\hat{k}
$$

Hitung:

$$
\begin{bmatrix}
3 \cdot 7 - 4 \cdot 6 \\
-(2 \cdot 7 - 4 \cdot 5) \\
2 \cdot 6 - 3 \cdot 5
\end{bmatrix} =
\begin{bmatrix}
21 - 24 \\
-(14 - 20) \\
12 - 15
\end{bmatrix} =
\begin{bmatrix}
-3 \\
6 \\
-3
\end{bmatrix}
$$


---

### Contoh 3

Misalkan:

$$
\mathbf{u} = \begin{bmatrix} 1 \\ 1 \\ 1 \end{bmatrix}, \quad
\mathbf{v} = \begin{bmatrix} 2 \\ 1 \\ 1 \end{bmatrix}
$$

<iframe src="https://www.geogebra.org/classic/khwmhesj" width="600" height="400" style="border:0;"></iframe>

$$
\mathbf{u} \times \mathbf{v} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3
\end{vmatrix}
= (u_2v_3 - u_3v_2)\hat{i} - (u_1v_3 - u_3v_1)\hat{j} + (u_1v_2 - u_2v_1)\hat{k}
$$

Hitung:

$$
\begin{bmatrix}
1 . 1 - 1 . 1 \\
-(1 . 1 - 1 . 2) \\
1 . 1 - 1 . 2
\end{bmatrix} = 
\begin{bmatrix}
0 \\ 1 \\ -1
\end{bmatrix}
$$

---

## Implementasi

### Luas Jajaran Genjang

Secara geometri, luas jajaran genjang adalah $A = b h$, di mana $b$ adalah panjang alas dan $h$ adalah tinggi jajaran genjang, seperti yang ditunjukkan dalam **Gambar (a)**.

Ketika kita mendefinisikan **aturan jajaran genjang penjumlahan vektor**, dua vektor $\vec{u}$ dan $\vec{v}$ membentuk jajaran genjang jika ditarik dari titik awal yang sama, seperti dalam **Gambar (b)**.

Trigonometri mengatakan bahwa $h = \|\vec{v}\| \sin(\theta)$, sehingga luas jajaran genjang adalah:

$$
A = \|\vec{u}\| \|\vec{v}\| \sin(\theta) = \|\vec{u} \times \vec{v}\|
$$

---

### Contoh

Tentukan luas jajaran genjang yang ditentukan oleh:

$$
\vec{u} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}, \quad
\vec{v} = \begin{bmatrix} 1 \\ 3 \end{bmatrix}
$$

Penyelesaiannya adalah dengan memandang $\vec{u}$ dan $\vec{v}$ sebagai vektor di bidang $xy$ dari $\mathbb{R}^3$, dan menulis ulang:

$$
\vec{u} = \begin{bmatrix} 2 \\ 1 \\ 0 \end{bmatrix}, \quad
\vec{v} = \begin{bmatrix} 1 \\ 3 \\ 0 \end{bmatrix}
$$

Kini kita dapat menghitung hasil kali silang:

$$
\vec{u} \times \vec{v} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
2 & 1 & 0 \\
1 & 3 & 0
\end{vmatrix} =
(1 \cdot 0 - 0 \cdot 3)\hat{i} - (2 \cdot 0 - 0 \cdot 1)\hat{j} + (2 \cdot 3 - 1 \cdot 1)\hat{k}
= \begin{bmatrix} 0 \\ 0 \\ 5 \end{bmatrix}
$$

Oleh karena itu:

$$
A = \|\vec{u} \times \vec{v}\| = 5
$$

---

## Volume Paralelepiped

**Paralelepiped** adalah bangun ruang tiga dimensi yang dibentuk oleh enam buah jajaran genjang.

Volume paralelepiped yang ditentukan oleh tiga vektor $\vec{u}, \vec{v}, \vec{w}$ diberikan oleh:

$$
V = |\vec{u} \cdot (\vec{v} \times \vec{w})|
$$

---

### Contoh: Menghitung Volume Paralelepiped

Tentukan volume paralelepiped yang ditentukan oleh vektor:

$$
\vec{u} = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}, \quad
\vec{v} = \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix}, \quad
\vec{w} = \begin{bmatrix} 0 \\ 1 \\ 1 \end{bmatrix}
$$

Langkah pertama: Hitung $\vec{v} \times \vec{w}$

$$
\vec{v} \times \vec{w} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
1 & 1 & 0 \\
0 & 1 & 1
\end{vmatrix} =
(1 \cdot 1 - 0 \cdot 1)\hat{i} - (1 \cdot 1 - 0 \cdot 0)\hat{j} + (1 \cdot 1 - 1 \cdot 0)\hat{k}
= \begin{bmatrix} 1 \\ -1 \\ 1 \end{bmatrix}
$$

Kemudian, hitung:

$$
\vec{u} \cdot (\vec{v} \times \vec{w}) = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ -1 \\ 1 \end{bmatrix} = 1
$$

Oleh karena itu:

$$
V = |\vec{u} \cdot (\vec{v} \times \vec{w})| = |1| = 1 \quad \text{satuan kubik}
$$

---

## Tugas Penyelesaian Soal

---

### Soal 1

Tentukan luas jajaran genjang yang ditentukan oleh vektor $\vec{u} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}$ dan $\vec{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}$.

### Penyelesaian:
Untuk $\mathbb{R}^2$, luas jajaran genjang diberikan oleh:

$$
L = |\vec{u} \times \vec{v}| = |u_1 v_2 - u_2 v_1|
$$

Substitusikan nilai:

$$
L = |1 \cdot 1 - 2 \cdot 2| = |1 - 4| = |-3| = 3
$$

**Jawaban: Luas = 3**

---

### Soal 2

Tentukan luas jajaran genjang yang ditentukan oleh vektor $\vec{u} = \begin{bmatrix} 2 \\ 0 \end{bmatrix}$ dan $\vec{v} = \begin{bmatrix} 0 \\ 3 \end{bmatrix}$.

### Penyelesaian:
Untuk $\mathbb{R}^2$, luas jajaran genjang diberikan oleh:

$$
L = |\vec{u} \times \vec{v}| = |u_1 v_2 - u_2 v_1|
$$

Substitusikan nilai:

$$
L = |u_1 v_2 - u_2 v_1| = |2 \cdot 3 - 0 \cdot 0| = |6 - 0| = 6
$$

**Jawaban: Luas = 6**

---

### Soal 3

Tentukan luas segitiga dengan titik-titik sudut (0, 0, 0), (1, 3, -1), dan (2, 1, 1).

### Penyelesaian:

Vektor $\vec{AB} = B - A = \langle 1, 3, -1 \rangle$  
Vektor $\vec{AC} = C - A = \langle 2, 1, 1 \rangle$

Hitung perkalian silang:

$$
\vec{AB} \times \vec{AC} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
1 & 3 & -1 \\
2 & 1 & 1
\end{vmatrix}
= (3 \cdot 1 - (-1) \cdot 1)\hat{i} - (1 \cdot 1 - (-1) \cdot 2)\hat{j} + (1 \cdot 1 - 3 \cdot 2)\hat{k}
$$
$$
= (3 + 1)\hat{i} - (1 + 2)\hat{j} + (1 - 6)\hat{k} = 4\hat{i} - 3\hat{j} - 5\hat{k}
$$

Luas segitiga:

$$
L = \frac{1}{2} \left\| \vec{AB} \times \vec{AC} \right\| = \frac{1}{2} \sqrt{4^2 + (-3)^2 + (-5)^2} = \frac{1}{2} \sqrt{16 + 9 + 25} = \frac{1}{2} \sqrt{50} = \frac{5\sqrt{2}}{1}
$$

**Jawaban: Luas = $\frac{5\sqrt{2}}{1}$**

---

### Soal 4

Tentukan luas segitiga dengan titik-titik sudut (5, 2, -1), (3, 6, 2), dan (1, 0, 4)

### Penyelesaian:

$\vec{AB} = B - A = \langle -2, 4, 3 \rangle$  
$\vec{AC} = C - A = \langle -4, -2, 5 \rangle$

Perkalian silang:

$$
\vec{AB} \times \vec{AC} =
\begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
-2 & 4 & 3 \\
-4 & -2 & 5
\end{vmatrix}
= (4 \cdot 5 - 3 \cdot (-2))\hat{i} - (-2 \cdot 5 - 3 \cdot (-4))\hat{j} + (-2 \cdot (-2) - 4 \cdot (-4))\hat{k}
$$
$$
= (20 + 6)\hat{i} - (-10 + 12)\hat{j} + (4 + 16)\hat{k}
= 26\hat{i} - 2\hat{j} + 20\hat{k}
$$

Luas segitiga:

$$
L = \frac{1}{2} \left\| \vec{AB} \times \vec{AC} \right\| = \frac{1}{2} \sqrt{26^2 + (-2)^2 + 20^2}
= \frac{1}{2} \sqrt{676 + 4 + 400} = \frac{1}{2} \sqrt{1080}
= \frac{\sqrt{1080}}{2}
$$

Sederhanakan:

$$
\sqrt{1080} = \sqrt{36 \cdot 30} = 6\sqrt{30}
$$

**Jawaban: Luas = $3\sqrt{30}$**