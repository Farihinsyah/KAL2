---
title: Perkalian Titik (Dot Product)

---

# Perkalian Titik (Dot Product)

## Pengertian Dot Product
Perkalian Titik (Dot Product) adalah operasi antara dua vektor yang menghasilkan skalar
Perkalian titik (dot product) dari dua vektor $\mathbf{v}$ dan $\mathbf{w}$ didefinisikan sebagai:

$$
\mathbf{v} \cdot \mathbf{w} =
\begin{bmatrix}
v_1 \\
v_2
\end{bmatrix}
\cdot
\begin{bmatrix}
w_1 \\
w_2
\end{bmatrix}
= v_1 w_1 + v_2 w_2
$$

---

### Operasi Dasar Vektor:

### Contoh 1:

<iframe src="https://www.geogebra.org/classic/x2spubbz" width="600" height="400" style="border:0;"></iframe>

Misalkan:

$$
\mathbf{u} = \begin{bmatrix} 3 \\ 0 \end{bmatrix}, \quad
\mathbf{v} = \begin{bmatrix} 2 \\ 4 \end{bmatrix}
$$

Hitung:

$$
\mathbf{u} \cdot \mathbf{v} = (3)(2) + (0)(4) = 6 + 0 = 6
$$

Karena hasilnya $\mathbf{u} \cdot \mathbf{v} = 6 \neq 0$, maka vektor $\mathbf{u}$ dan $\mathbf{v}$ *tidak ortogonal* (tidak tegak lurus).

---

### Contoh 2:

<iframe src="https://www.geogebra.org/classic/qvzjecxt" width="600" height="400" style="border:0;"></iframe>

Misalkan:

$$
\mathbf{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}, \quad
\mathbf{w} = \begin{bmatrix} -1 \\ 2 \end{bmatrix}
$$

Maka:

$$
\mathbf{v} \cdot \mathbf{w} = (2)(-1) + (1)(2) = -2 + 2 = 0
$$

Karena hasilnya $0$, maka **vektor $\mathbf{v}$ dan $\mathbf{w}$ saling tegak lurus (ortogonal)**.

---

### Contoh 3:

<iframe src="https://www.geogebra.org/classic/wzcskt4h" width="600" height="400" style="border:0;"></iframe>

Misalkan:

$$
\mathbf{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}, \quad
\mathbf{w} = \begin{bmatrix} -2 \\ 4 \end{bmatrix}
$$

Maka:

$$
\mathbf{v} \cdot \mathbf{w} = (2)(-2) + (1)(4) = -4 + 4 = 0
$$

Hasilnya juga $0$, sehingga **vektor $\mathbf{v}$ dan $\mathbf{w}$ juga ortogonal**, meskipun nilai komponennya berbeda dari contoh sebelumnya.

---

### Kesimpulan:

Jika hasil dot product antara dua vektor adalah nol:

$$
\mathbf{v} \cdot \mathbf{w} = 0
$$

Maka vektor $\mathbf{v}$ dan $\mathbf{w}$ dipastikan saling tegak lurus.
