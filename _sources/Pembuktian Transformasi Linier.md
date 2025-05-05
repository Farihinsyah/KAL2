---
title: Pembuktian Transformasi Linier

---

## Pembuktian Transformasi Linier

Diberikan transformasi:

$$
T(v_1, v_2) = (v_1 + v_2, v_1)
$$

Kita ingin membuktikan bahwa $T$ adalah transformasi linier. Untuk itu, kita harus menunjukkan bahwa $T$ memenuhi dua sifat berikut untuk semua vektor $\mathbf{u}, \mathbf{v} \in \mathbb{R}^2$ dan semua skalar $c \in \mathbb{R}$:

---

### **1. Sifat Additivitas (Penjumlahan Vektor)**

Syarat:

$$
T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})
$$

Misalkan:

$$
\mathbf{u} = (u_1, u_2), \quad \mathbf{v} = (v_1, v_2)
$$

Maka:

$$
\mathbf{u} + \mathbf{v} = (u_1 + v_1, u_2 + v_2)
$$

Hitung sisi kiri:

$$
T(\mathbf{u} + \mathbf{v}) = T(u_1 + v_1, u_2 + v_2)
= \left((u_1 + v_1) + (u_2 + v_2),\ u_1 + v_1\right)
= \left(u_1 + u_2 + v_1 + v_2,\ u_1 + v_1\right)
$$

Hitung sisi kanan:

- $T(\mathbf{u}) = (u_1 + u_2, u_1)$  
- $T(\mathbf{v}) = (v_1 + v_2, v_1)$

Maka:

$$
T(\mathbf{u}) + T(\mathbf{v}) 
= (u_1 + u_2 + v_1 + v_2,\ u_1 + v_1)
$$

Karena:

$$
T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})
$$

maka sifat **additivitas terpenuhi**.

---

### **2. Sifat Homogenitas (Perkalian Skalar)**

Syarat:

$$
T(c\mathbf{u}) = cT(\mathbf{u})
$$

Misalkan $\mathbf{u} = (u_1, u_2)$ dan $c$ adalah skalar.

Hitung sisi kiri:

$$
c\mathbf{u} = (cu_1, cu_2)
$$

$$
T(c\mathbf{u}) = T(cu_1, cu_2)
= (cu_1 + cu_2,\ cu_1)
= c(u_1 + u_2,\ u_1)
$$

Hitung sisi kanan:

$$
T(\mathbf{u}) = (u_1 + u_2,\ u_1)
$$

$$
cT(\mathbf{u}) = c(u_1 + u_2,\ u_1) = (cu_1 + cu_2,\ cu_1)
$$

Karena:

$$
T(c\mathbf{u}) = cT(\mathbf{u})
$$

maka sifat **homogenitas terpenuhi**.

---

### **Kesimpulan**

Karena transformasi $T$ memenuhi kedua sifat:

- Penjumlahan vektor: $T(\mathbf{u} + \mathbf{v}) = T(\mathbf{u}) + T(\mathbf{v})$
- Perkalian skalar: $T(c\mathbf{u}) = cT(\mathbf{u})$

maka kita simpulkan bahwa:

$$
\boxed{T(v_1, v_2) = (v_1 + v_2, v_1) \text{ adalah transformasi linier}}
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
- $B(-1, -4) \rightarrow B'(-1, 4)$

---

### 2. Refleksi terhadap sumbu-$y$

Matriks transformasi:

$$
\begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}
$$

Contoh titik:

- $C(3, 2) \rightarrow C'(-3, 2)$  
- $D(-2, -1) \rightarrow D'(2, -1)$

---

### 3. Refleksi terhadap garis $y = x$

Matriks transformasi:

$$
\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}
$$

Contoh titik:

- $E(1, 4) \rightarrow E'(4, 1)$  
- $F(-3, 2) \rightarrow F'(2, -3)$

---

### 4. Refleksi terhadap garis $y = -x$

Matriks transformasi:

$$
\begin{bmatrix} 0 & -1 \\ -1 & 0 \end{bmatrix}
$$

Contoh titik:

- $G(2, 5) \rightarrow G'(-5, -2)$  
- $H(-1, -4) \rightarrow H'(4, 1)$

---

### 5. Refleksi terhadap titik asal (origin)

Matriks transformasi:

$$
\begin{bmatrix} -1 & 0 \\ 0 & -1 \end{bmatrix}
$$

Contoh titik:

- $I(3, -2) \rightarrow I'(-3, 2)$  
- $J(-5, 1) \rightarrow J'(5, -1)$
