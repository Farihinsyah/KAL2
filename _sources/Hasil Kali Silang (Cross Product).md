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


## Sifat-sifat:
- $\vec{a} \times \vec{b} = -(\vec{b} \times \vec{a})$
- Jika $\vec{a}$ dan $\vec{b}$ sejajar, maka $\vec{a} \times \vec{b} = \vec{0}$
- $\vec{a} \times \vec{a} = \vec{0}$
- $|\vec{a} \times \vec{b}| = |\vec{a}||\vec{b}|\sin\theta$

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
\end{bmatrix}
$$

$$
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
\end{bmatrix}
$$

$$
\begin{bmatrix}
21 - 24 \\
-(14 - 20) \\
12 - 15
\end{bmatrix}
$$

$$
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

## Penyelesaian Soal 1 – Luas Jajaran Genjang dan Segitiga

---

### Soal 1

Diketahui vektor $\vec{u} = \begin{bmatrix} 1 \\ 2 \end{bmatrix}$ dan $\vec{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}$.

Hitunglah luas jajaran genjang yang dibentuk oleh kedua vektor tersebut.

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

Diketahui $\vec{u} = \begin{bmatrix} 2 \\ 0 \end{bmatrix}$ dan $\vec{v} = \begin{bmatrix} 0 \\ 3 \end{bmatrix}$.

### Penyelesaian:
$$
L = |u_1 v_2 - u_2 v_1| = |2 \cdot 3 - 0 \cdot 0| = |6 - 0| = 6
$$

**Jawaban: Luas = 6**

---

### Soal 3

Diketahui tiga titik sudut segitiga: $A = (0, 0, 0)$, $B = (1, 3, -1)$, dan $C = (2, 1, 1)$.

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

Diketahui titik-titik: $A = (5, 2, -1)$, $B = (3, 6, 2)$, $C = (1, 0, 4)$

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