---
title: Eigenvalues Eigenvectors

---

# Eigenvalues Eigenvectors

## Definisi Eigenvalues dan Eigenvectors

Persamaan utama:

$$
A\mathbf{v} = \lambda \mathbf{v}
$$

- **Eigenvalues ($\lambda$)**: Menunjukkan berapa besar perubahan skala yang terjadi pada vektor setelah dikalikan dengan matriks $A$.
- **Eigenvectors ($\mathbf{v}$)**: Arah khusus yang tidak berubah arah setelah dikalikan dengan matriks $A$, hanya memanjang atau memendek (dikali skalar $\lambda$).

## Mencari Eigenvalues dan Eigenvectors

```python
import numpy as np
A = np.array([[2,1],[1,2]])
eigenvalues, eigenvectors = np.linalg.eig(A)
print(A)
print("\neigenvalues")
print(eigenvalues)
print("\neigenvectors")
print(eigenvectors)
```
```python
[[2 1]
 [1 2]]

eigenvalues
[3. 1.]

eigenvectors
[[ 0.70710678 -0.70710678]
 [ 0.70710678  0.70710678]]
```
```python
import numpy as np
A = np.array([[8, -10], [5, -7]])
eigenvalues, eigenvectors = np.linalg.eig(A)
print(A)
print("\neigenvalues")
print(eigenvalues)
print("\neigenvectors")
print(eigenvectors)
```
```python
[[8 -10]
 [5  -7]]

eigenvalues
[3. -2.]

eigenvectors
[[ 0.89442719  0.70710678]
 [ 0.4472136  -0.70710678]]
```

## Definisi Vektor Ortogonal dan Vektor Ortonormal

- **Vektor Ortogonal**: Terdiri dari dua vektor, dan kedua vektor saling tegak lurus
- **Vektor Ortonormal**: Saling ortogonal (tegak lurus), dan Normanya panjangnya = 1



## Contoh Vektor Ortogonal dan Ortonormal


### 1. Mencari Nilai Eigen (Eigenvalue)

Diketahui matriks:

$$
A = \begin{bmatrix} 5 & 2 \\ 2 & 5 \end{bmatrix}
$$

Untuk mencari nilai eigen ($\lambda$), digunakan persamaan karakteristik:

$$
\det(A - \lambda I) = 0
$$

$$
\det
\begin{bmatrix}
5 - \lambda & 2 \\
2 & 5 - \lambda
\end{bmatrix}
= (5 - \lambda)^2 - (2)(2)
$$

$$
= (5 - \lambda)^2 - 4
$$

$$
= 25 - 10\lambda + \lambda^2 - 4
$$

$$
= \lambda^2 - 10\lambda + 21
$$

$$
\lambda^2 - 10\lambda + 21 = 0
$$

$$
(\lambda - 3)(\lambda - 7) = 0
$$

$$
\lambda_1 = 3, \quad \lambda_2 = 7
$$

---

### 2. Mencari Vektor Eigen (Eigenvector)

Gunakan $(A - \lambda I)\mathbf{v} = 0$

#### Untuk $\lambda = 3$:

Kurangkan:

$$
A - 3I = \begin{bmatrix} 2 & 2 \\ 2 & 2 \end{bmatrix}
$$

Maka sistem persamaan:

$$
\begin{cases}
2x + 2y = 0 \\
2x + 2y = 0
\end{cases}
\Rightarrow x = -y
$$

Pilih vektor bebas: $\mathbf{v}_1 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}$

---

#### Untuk $\lambda = 7$:

Kurangkan:

$$
A - 7I = \begin{bmatrix} -2 & 2 \\ 2 & -2 \end{bmatrix}
$$

Maka sistem persamaan:

$$
\begin{cases}
-2x + 2y = 0 \\
2x - 2y = 0
\end{cases}
\Rightarrow x = y
$$

Pilih vektor bebas: $\mathbf{v}_2 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}$

---

### 3. Mengecek Ortogonalitas

Dua vektor ortogonal jika dot product-nya nol:

$$
\mathbf{v}_1 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}, \quad
\mathbf{v}_2 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}
$$

$$
\mathbf{v}_1 \cdot \mathbf{v}_2
= (1 \times 1) + (-1 \times 1) = 1 - 1 = 0
$$

Jadi, $\mathbf{v}_1$ dan $\mathbf{v}_2$ **ortogonal**

---

### 4. Menjadikan Vektor Ortonormal

Hitung norma (panjang) masing-masing:

$$
\|\mathbf{v}_1\| = \sqrt{1^2 + (-1)^2} = \sqrt{2},\quad
\|\mathbf{v}_2\| = \sqrt{1^2 + 1^2} = \sqrt{2}
$$

Normalisasi (bagi dengan panjang):

$$
\mathbf{u}_1 = \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -1 \end{bmatrix},\quad
\mathbf{u}_2 = \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ 1 \end{bmatrix}
$$