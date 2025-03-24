---
title: Menghitung Invers Matrik

---

# Menghitung Invers Matrik

Membuat persamaan 3 variabel

$$\begin{aligned}
4x+2y+6z=4 \\
6x+2y+3z=6 \\
2x+4y+2z=2
\end{aligned}$$

Langkah 1 : Tuliskan dalam Bentuk Matriks Augmented
$$\begin{bmatrix}
4 & 2 & 6 & 1 & 0 & 0 \\
6 & 2 & 3 & 0 & 1 & 0 \\
2 & 4 & 2 & 0 & 0 & 1
\end{bmatrix}$$

Langkah 2 : Baris pertama dibagi 4:
$$\begin{bmatrix}
1 & \frac{1}{2} & \frac{3}{2} & \frac{1}{4} & 0 & 0 \\
6 & 2 & 3 & 0 & 1 & 0 \\
2 & 4 & 2 & 0 & 0 & 1
\end{bmatrix}$$

Langkah 3 : R2 = R2 - 6R1 dan R3 = R3 - 2R1
$$\begin{bmatrix}
1 & \frac{1}{2} & \frac{3}{2} & \frac{1}{4} & 0 & 0 \\
0 & -1 & -6 & -\frac{3}{2} & 1 & 0 \\
0 & 3 & -1 & -\frac{1}{2} & 0 & 1
\end{bmatrix}$$

Langkah 4 : R2 = R2 : -1
$$\begin{bmatrix}
1 & \frac{1}{2} & \frac{3}{2} & \frac{1}{4} & 0 & 0 \\
0 & 1 & 6 & \frac{3}{2} & -1 & 0 \\
0 & 3 & -1 & -\frac{1}{2} & 0 & 1
\end{bmatrix}$$

Langkah 5 : R1 = R1 - $\frac{1}{2}$ R2 dan R3 = R3 - 3R2
$$\begin{bmatrix}
1 & 0 & -2 & -\frac{1}{2} & \frac{1}{2} & 0 \\
0 & 1 & 6 & \frac{3}{2} & -1 & 0 \\
0 & 0 & -19 & -5 & 3 & 1
\end{bmatrix}$$

Langkah 6 : R3 = R3 : -19
$$\begin{bmatrix}
1 & 0 & -2 & -\frac{1}{2} & \frac{1}{2} & 0 \\
0 & 1 & 6 & \frac{3}{2} & -1 & 0 \\
0 & 0 & 1 & \frac{5}{19} & -\frac{3}{19} & -\frac{1}{19}
\end{bmatrix}$$

Langkah 7 : R1 = R1 + 2R3 dan R2 = R2 - 6R3
$$\begin{bmatrix}
1 & 0 & 0 & -\frac{9}{19} & \frac{8}{19} & \frac{2}{19} \\
0 & 1 & 0 & \frac{3}{19} & -\frac{3}{19} & \frac{6}{19} \\
0 & 0 & 1 & \frac{5}{19} & -\frac{3}{19} & -\frac{1}{19}
\end{bmatrix}$$

Penyelesaian
$$
\begin{vmatrix} x1 \\ x2 \\ x3\end{vmatrix} =
\begin{vmatrix} -\frac{9}{19} & \frac{8}{19} & \frac{2}{19} \\ \frac{3}{19} & -\frac{3}{19} & \frac{6}{19} \\ \frac{5}{19} & -\frac{3}{19} & -\frac{1}{19}\end{vmatrix}
\begin{vmatrix} 4 \\ 6 \\ 2\end{vmatrix} =
\begin{vmatrix} 0,842 \\ 0,3158 \\ 0\end{vmatrix} =
\begin{vmatrix} 1 \\ 0 \\ 0\end{vmatrix}
$$
