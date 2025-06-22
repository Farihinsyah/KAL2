---
title: Singular Value Decomposition

---

# Singular Value Decomposition (SVD)

## Pengertian

**SVD** (Singular Value Decomposition) adalah teknik faktorisasi matriks yang menyatakan suatu matriks $A$ menjadi hasil perkalian tiga matriks:

$$
A = U \Sigma V^T
$$

Dengan:

- $A$: matriks asli berukuran $m \times n$
- $U$: matriks ortogonal berukuran $m \times m$
- $\Sigma$: matriks diagonal berukuran $m \times n$ dengan entri non-negatif
- $V^T$: transpose dari matriks ortogonal $V$ berukuran $n \times n$

---

## Komponen Matriks SVD

- **$U$**: Kolom-kolomnya disebut *left singular vectors* (vektor singular kiri), merupakan basis ortonormal dari ruang kolom $A$.
- **$\Sigma$**: Matriks diagonal dengan nilai-nilai singular (singular values) $\sigma_1 \geq \sigma_2 \geq \dots \geq \sigma_r > 0$ pada diagonal utama.
- **$V$**: Kolom-kolomnya disebut *right singular vectors* (vektor singular kanan), merupakan basis ortonormal dari ruang baris $A$.

---

## Kegunaan SVD

1. **Kompresi data**: menyimpan informasi utama dengan membuang nilai singular kecil.
2. **Reduksi dimensi** (PCA - Principal Component Analysis)
3. **Sistem rekomendasi**: digunakan pada user-item matrix seperti di Netflix atau Spotify.
4. **Penyelesaian sistem persamaan linear**: cocok untuk sistem yang over/under-determined.
5. **Pengurangan noise**: dengan membuang komponen kecil dari $\Sigma$.
6. **Kompresi gambar**: menyimpan gambar dalam ukuran kecil dengan kualitas yang masih tinggi.

---

## Contoh 1

Diketahui matriks:  
$A = \begin{bmatrix} 3 & 1 \\ 1 & 3 \end{bmatrix}$

Kita ingin mencari faktorisasi:  
$A = U \Sigma V^T$

---

### Langkah 1: Hitung $A^T A$

Karena $A$ simetris, maka:

$A^T A = A A^T$ =
$$
\begin{bmatrix} 3 & 1 \\ 1 & 3 \end{bmatrix}
\begin{bmatrix} 3 & 1 \\ 1 & 3 \end{bmatrix} =
\begin{bmatrix} 10 & 6 \\ 6 & 10 \end{bmatrix}
$$

---

### Langkah 2: Cari nilai eigen $\lambda$ dari $A^T A$

Gunakan determinan:  
$\det \left( A^T A - \lambda I \right) = 0$

$\left|
\begin{matrix}
10 - \lambda & 6 \\
6 & 10 - \lambda
\end{matrix}
\right| = (10 - \lambda)^2 - 36 = 0$

$(10 - \lambda)^2 = 36 \Rightarrow 10 - \lambda = \pm 6  
\Rightarrow \lambda_1 = 16, \quad \lambda_2 = 4$

---

### Langkah 3: Cari nilai singular

$\sigma_1 = \sqrt{16} = 4, \quad \sigma_2 = \sqrt{4} = 2$

Maka matriks $\Sigma$ adalah:  
$\Sigma = \begin{bmatrix}
4 & 0 \\
0 & 2
\end{bmatrix}$

---

### Langkah 4: Cari vektor eigen untuk $V$

Untuk $\lambda_1 = 16$:  
$(A^T A - 16I)v = 0 \Rightarrow 
\begin{bmatrix} -6 & 6 \\ 6 & -6 \end{bmatrix}
\Rightarrow v_1 = \begin{bmatrix} 1 \\ 1 \end{bmatrix}  
\Rightarrow \hat{v}_1 = \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ 1 \end{bmatrix}$

Untuk $\lambda_2 = 4$:  
$(A^T A - 4I)v = 0 \Rightarrow 
\begin{bmatrix} 6 & 6 \\ 6 & 6 \end{bmatrix}
\Rightarrow v_2 = \begin{bmatrix} 1 \\ -1 \end{bmatrix}  
\Rightarrow \hat{v}_2 = \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -1 \end{bmatrix}$

Maka:  
$V = \begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix}$

---

### Langkah 5: Hitung $U$ dari rumus:

$u_i = \frac{1}{\sigma_i} A v_i$

Untuk $u_1$:  
$u_1 = \frac{1}{4} A \left( \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ 1 \end{bmatrix} \right)
= \frac{1}{4\sqrt{2}} \begin{bmatrix} 3 + 1 \\ 1 + 3 \end{bmatrix}
= \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ 1 \end{bmatrix}$

Untuk $u_2$:  
$u_2 = \frac{1}{2} A \left( \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -1 \end{bmatrix} \right)
= \frac{1}{2\sqrt{2}} \begin{bmatrix} 3 - 1 \\ 1 - 3 \end{bmatrix}
= \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -1 \end{bmatrix}$

Maka:  
$U = \begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix}$

---

### Jawaban Akhir:

$A = U \Sigma V^T$

Dengan:

- $U = \begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix}$

- $\Sigma = \begin{bmatrix}
4 & 0 \\
0 & 2
\end{bmatrix}$

- $V^T = \begin{bmatrix}
\frac{1}{\sqrt{2}} & \frac{1}{\sqrt{2}} \\
\frac{1}{\sqrt{2}} & -\frac{1}{\sqrt{2}}
\end{bmatrix}$

---

## Contoh 2

Diketahui matriks:

$A = \begin{bmatrix} 4 & 1 \\ 2 & 7 \\ 1 & 4 \end{bmatrix}$

Kita ingin mencari faktorisasi SVD:

$A = U \Sigma V^T$

---

### Langkah 1: Hitung $A^T A$

$A^T A$ =

$$
\begin{bmatrix} 4 & 2 & 1 \\ 1 & 7 & 4 \end{bmatrix}
\begin{bmatrix} 4 & 1 \\ 2 & 7 \\ 1 & 4 \end{bmatrix} = 
\begin{bmatrix} 21 & 18 \\ 18 & 66 \end{bmatrix}
$$

---

### Langkah 2: Cari eigenvalue $\lambda$ dari $A^T A$

$\det(A^T A - \lambda I) = 0$

$\left|
\begin{matrix}
21 - \lambda & 18 \\
18 & 66 - \lambda
\end{matrix}
\right| = (21 - \lambda)(66 - \lambda) - 324 = 0$

Hitung:

$\lambda^2 - 87\lambda + (1386 - 324) = \lambda^2 - 87\lambda + 1062 = 0$

Gunakan rumus kuadrat:

$\lambda = \frac{87 \pm \sqrt{87^2 - 4 \cdot 1062}}{2} = \frac{87 \pm \sqrt{7569 - 4248}}{2} = \frac{87 \pm \sqrt{3321}}{2}$

$\Rightarrow \lambda_1 \approx 72.3,\quad \lambda_2 \approx 14.7$

---

### Langkah 3: Nilai singular

$\sigma_1 = \sqrt{72.3} \approx 8.5,\quad \sigma_2 = \sqrt{14.7} \approx 3.8$

Maka matriks $\Sigma$ berukuran $3 \times 2$ adalah:

$\Sigma = \begin{bmatrix}
8.5 & 0 \\
0 & 3.8 \\
0 & 0
\end{bmatrix}$

---

### Langkah 4: Cari vektor eigen untuk $V$

Gunakan nilai eigen $\lambda$ untuk mencari vektor eigen dari $A^T A$.

Untuk $\lambda_1 \approx 72.3$, kita peroleh vektor eigen:

$v_1 \approx \begin{bmatrix} 0.316 \\ 0.949 \end{bmatrix}$

Untuk $\lambda_2 \approx 14.7$, diperoleh vektor eigen ortonormal:

$v_2 \approx \begin{bmatrix} 0.949 \\ -0.316 \end{bmatrix}$

Sehingga matriks $V$ adalah:

$V = \begin{bmatrix}
0.316 & 0.949 \\
0.949 & -0.316
\end{bmatrix}$

---

### Langkah 5: Hitung $U$ dari rumus

$u_i = \frac{1}{\sigma_i} A v_i$

Misalnya:

$u_1 = \frac{1}{8.5} A v_1 \Rightarrow u_1 \approx \begin{bmatrix} 0.428 \\ 0.667 \\ 0.607 \end{bmatrix}$

$u_2 = \frac{1}{3.8} A v_2 \Rightarrow u_2 \approx \begin{bmatrix} -0.562 \\ 0.430 \\ -0.705 \end{bmatrix}$

Lengkapi $U$ menjadi ortonormal $3 \times 3$ (misalnya dengan Gram-Schmidt), tapi untuk SVD, hanya dua kolom pertama yang dipakai.

---

### Jawaban Akhir:

$A = U \Sigma V^T$

Dengan:

- $U \approx \begin{bmatrix}
0.428 & -0.562 & u_3 \\
0.667 &  0.430 & u_3 \\
0.607 & -0.705 & u_3
\end{bmatrix}$

- $\Sigma = \begin{bmatrix}
8.5 & 0 \\
0 & 3.8 \\
0 & 0
\end{bmatrix}$

- $V^T = \begin{bmatrix}
0.316 & 0.949 \\
0.949 & -0.316
\end{bmatrix}$
