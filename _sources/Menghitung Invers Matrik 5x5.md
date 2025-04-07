---
title: Menghitung Invers Matrik 5x5

---

# Menghitung Invers Matrik 5x5

Membuat 5 persamaan 5 variabel

$$\begin{aligned}
2x1+2x2-2x3+4x4+6x5=2 \\
6x1-2x2-2x3+6x4+4x5=6 \\
4x1-4x2+5x3+6x4+2x5=4 \\
3x1+3x2+6x3+5x4-5x5=3 \\
x1+4x2-3x3+4x4+x5=1
\end{aligned}$$

Tuliskan dalam Bentuk Matriks Augmented

$$
\left[
\begin{array}{ccccc|cc}
2 & 2 & -2 & 4 & 6 & 1 & 0 & 0 & 0 & 0 \\
6 & -2 & -2 & 6 & 4 & 0 & 1 & 0 & 0 & 0 \\
4 & -4 & 5 & 6 & 2 & 0 & 0 & 1 & 0 & 0 \\
3 & 3 & 6 & 5 & -5 & 0 & 0 & 0 & 1 & 0 \\
1 & 4 & -3 & 4 & 1 & 0 & 0 & 0 & 0 & 1
\end{array}
\right]
$$

Langkah 1 :
R1 x $\frac{1}{2}$

$$
\left[
\begin{array}{ccccc|cc}
1 & 1 & -1 & 2 & 3 & \frac{1}{2} & 0 & 0 & 0 & 0 \\
6 & -2 & -2 & 6 & 4 & 0 & 1 & 0 & 0 & 0 \\
4 & -4 & 5 & 6 & 2 & 0 & 0 & 1 & 0 & 0 \\
3 & 3 & 6 & 5 & -5 & 0 & 0 & 0 & 1 & 0 \\
1 & 4 & -3 & 4 & 1 & 0 & 0 & 0 & 0 & 1
\end{array}
\right]
$$

Langkah 2 :
R2 - 6R1
R3 - 4R1
R4 - 3R1
R5 - 1R1

$$
\left[
\begin{array}{ccccc|cc}
1 & 1 & -1 & 2 & 3 & \frac{1}{2} & 0 & 0 & 0 & 0 \\
0 & -8 & 4 & -6 & -14 & -3 & 1 & 0 & 0 & 0 \\
0 & -8 & 9 & -2 & -10 & -2 & 0 & 1 & 0 & 0 \\
0 & 0 & 9 & -1 & -14 & -\frac{3}{2} & 0 & 0 & 1 & 0 \\
0 & 3 & -2 & 2 & -2 & -\frac{1}{2} & 0 & 0 & 0 & 1
\end{array}
\right]
$$

Langkah 3 : 
R2 x $\frac{1}{-8}$

$$
\left[
\begin{array}{ccccc|cc}
1 & 1 & -1 & 2 & 3 & \frac{1}{2} & 0 & 0 & 0 & 0 \\
0 & 1 & -\frac{1}{2} & \frac{3}{4} & \frac{7}{4} & \frac{3}{8} & -\frac{1}{8} & 0 & 0 & 0 \\
0 & -8 & 9 & -2 & -10 & -2 & 0 & 1 & 0 & 0 \\
0 & 0 & 9 & -1 & -14 & -\frac{3}{2} & 0 & 0 & 1 & 0 \\
0 & 3 & -2 & 2 & -2 & -\frac{1}{2} & 0 & 0 & 0 & 1
\end{array}
\right]
$$

Langkah 4 :
R1 - 1R2
R3 + 8R2
R5 - 3R2

$$
\left[
\begin{array}{ccccc|cc}
1 & 0 & -\frac{1}{2} & \frac{5}{4} & \frac{5}{4} & \frac{1}{8} & \frac{1}{8} & 0 & 0 & 0 \\
0 & 1 & -\frac{1}{2} & \frac{3}{4} & \frac{7}{4} & \frac{3}{8} & -\frac{1}{8} & 0 & 0 & 0 \\
0 & 0 & 5 & 4 & 4 & 1 & -1 & 1 & 0 & 0 \\
0 & 0 & 9 & -1 & -14 & -\frac{3}{2} & 0 & 0 & 1 & 0 \\
0 & 0 & -\frac{1}{2} & -\frac{1}{4} & -\frac{29}{4} & -\frac{13}{8} & \frac{3}{8} & 0 & 0 & 1
\end{array}
\right]
$$

Langkah 5 :
R3 : 5

$$
\left[
\begin{array}{ccccc|cc}
1 & 0 & -\frac{1}{2} & \frac{5}{4} & \frac{5}{4} & \frac{1}{8} & \frac{1}{8} & 0 & 0 & 0 \\
0 & 1 & -\frac{1}{2} & \frac{3}{4} & \frac{7}{4} & \frac{3}{8} & -\frac{1}{8} & 0 & 0 & 0 \\
0 & 0 & 1 & \frac{4}{5} & \frac{4}{5} & \frac{1}{5} & -\frac{1}{5} & \frac{1}{5} & 0 & 0 \\
0 & 0 & 9 & -1 & -14 & -\frac{3}{2} & 0 & 0 & 1 & 0 \\
0 & 0 & -\frac{1}{2} & -\frac{1}{4} & -\frac{29}{4} & -\frac{13}{8} & \frac{3}{8} & 0 & 0 & 1
\end{array}
\right]
$$

Langkah 6 :
R1 + $\frac{1}{2}$R3
R2 + $\frac{1}{2}$R3
R4 - 9R3
R5 + $\frac{1}{2}$R3

$$
\left[
\begin{array}{ccccc|cc}
1 & 0 & 0 & \frac{33}{20} & \frac{33}{20} & \frac{9}{40} & \frac{1}{40} & \frac{1}{10} & 0 & 0 \\
0 & 1 & 0 & \frac{23}{20} & \frac{43}{20} & \frac{19}{40} & -\frac{9}{40} & \frac{1}{10} & 0 & 0 \\
0 & 0 & 1 & \frac{4}{5} & \frac{4}{5} & \frac{1}{5} & -\frac{1}{5} & \frac{1}{5} & 0 & 0 \\
0 & 0 & 0 & -\frac{41}{5} & -\frac{106}{5} & -\frac{33}{10} & \frac{9}{5} & -\frac{9}{5} & 1 & 0 \\
0 & 0 & 0 & \frac{3}{20} & -\frac{137}{20} & -\frac{61}{40} & \frac{11}{40} & \frac{1}{10} & 0 & 1
\end{array}
\right]
$$

Langkah 7 :
R4 x $\frac{5}{-41}$

$$
\left[
\begin{array}{ccccc|cc}
1 & 0 & 0 & \frac{33}{20} & \frac{33}{20} & \frac{9}{40} & \frac{1}{40} & \frac{1}{10} & 0 & 0 \\
0 & 1 & 0 & \frac{23}{20} & \frac{43}{20} & \frac{19}{40} & -\frac{9}{40} & \frac{1}{10} & 0 & 0 \\
0 & 0 & 1 & \frac{4}{5} & \frac{4}{5} & \frac{1}{5} & -\frac{1}{5} & \frac{1}{5} & 0 & 0 \\
0 & 0 & 0 & 1 & \frac{106}{41} & \frac{33}{82} & -\frac{9}{41} & \frac{9}{41} & -\frac{5}{41} & 0 \\
0 & 0 & 0 & \frac{3}{20} & -\frac{137}{20} & -\frac{61}{40} & \frac{11}{40} & \frac{1}{10} & 0 & 1
\end{array}
\right]
$$

Langkah 8 :
R1 - $\frac{33}{20}$R4
R2 - $\frac{23}{20}$R4
R3 - $\frac{4}{5}$R4
R5 - $\frac{3}{20}$R4

$$
\left[
\begin{array}{ccccc|cc}
1 & 0 & 0 & 0 & -\frac{429}{164} & -\frac{9}{41} & \frac{635}{1640} & -\frac{43}{164} & \frac{33}{164} & 0 \\
0 & 1 & 0 & 0 & -\frac{135}{164} & -\frac{739}{1640} & \frac{1701}{1640} & -\frac{25}{164} & \frac{23}{164} & 0 \\
0 & 0 & 1 & 0 & -\frac{52}{41} & -\frac{91}{205} & -\frac{1}{41} & \frac{1}{41} & \frac{4}{41} & 0 \\
0 & 0 & 0 & 1 & \frac{106}{41} & \frac{33}{82} & \frac{72}{41} & \frac{9}{41} & -\frac{5}{41} & 0 \\
0 & 0 & 0 & 0 & -\frac{5935}{820} & -\frac{2603}{1640} & \frac{505}{1640} & \frac{11}{164} & \frac{3}{164} & 1
\end{array}
\right]
$$


Langkah 9 :
R5 x $\frac{820}{-5935}$

$$
\left[
\begin{array}{ccccc|cc}
1 & 0 & 0 & 0 & -\frac{429}{164} & -\frac{9}{41} & \frac{635}{1640} & -\frac{43}{164} & \frac{33}{164} & 0 \\
0 & 1 & 0 & 0 & -\frac{135}{164} & -\frac{739}{1640} & \frac{1701}{1640} & -\frac{25}{164} & \frac{23}{164} & 0 \\
0 & 0 & 1 & 0 & -\frac{52}{41} & -\frac{91}{205} & -\frac{1}{41} & \frac{1}{41} & \frac{4}{41} & 0 \\
0 & 0 & 0 & 1 & \frac{106}{41} & \frac{33}{82} & \frac{72}{41} & \frac{9}{41} & -\frac{5}{41} & 0 \\
0 & 0 & 0 & 0 & 1 & \frac{2603}{11870} & -\frac{101}{2374} & -\frac{11}{1187} & -\frac{3}{1187} & -\frac{164}{1187}
\end{array}
\right]
$$

Langkah 10 :
R1 + $\frac{429}{164}$R5
R2 + $\frac{135}{164}$R5
R3 + $\frac{52}{41}$R5
R4 - $\frac{106}{41}$R5

$$
\left[
\begin{array}{ccccc|cc}
1 & 0 & 0 & 0 & 0 & \frac{689367}{1946680} & \frac{655}{2374} & -\frac{340}{1187} & \frac{231}{1187} & -\frac{429}{1187} \\
0 & 1 & 0 & 0 & 0 & -\frac{131447}{486670} & \frac{243864}{243335} & -\frac{190}{1187} & \frac{164}{1187} & -\frac{135}{1187} \\
0 & 0 & 1 & 0 & 0 & -\frac{40339}{243335} & -\frac{93}{1187} & \frac{15}{1187} & \frac{112}{1187} & -\frac{208}{1187} \\
0 & 0 & 0 & 1 & 0 & -\frac{80063}{486670} & \frac{90817}{48667} & \frac{289}{1187} & -\frac{137}{1187} & \frac{424}{1187} \\
0 & 0 & 0 & 0 & 1 & \frac{2603}{11870} & -\frac{101}{2374} & -\frac{11}{1187} & -\frac{3}{1187} & -\frac{164}{1187}
\end{array}
\right]
$$

Penyelesaian


$\begin{vmatrix} x1 \\ x2 \\ x3 \\ x4 \\ x5\end{vmatrix} =
\begin{vmatrix} \frac{689367}{1946680} & \frac{655}{2374} & -\frac{340}{1187} & \frac{231}{1187} & -\frac{429}{1187} \\ -\frac{131447}{486670} & \frac{243864}{243335} & -\frac{190}{1187} & \frac{164}{1187} & -\frac{135}{1187} \\ -\frac{40339}{243335} & -\frac{93}{1187} & \frac{15}{1187} & \frac{112}{1187} & -\frac{208}{1187} \\ -\frac{80063}{486670} & \frac{90817}{48667} & \frac{289}{1187} & -\frac{137}{1187} & \frac{424}{1187} \\ \frac{2603}{11870} & -\frac{101}{2374} & -\frac{11}{1187} & -\frac{3}{1187} & -\frac{164}{1187}\end{vmatrix}
\begin{vmatrix} 2 \\ 6 \\ 4 \\ 3 \\ 1\end{vmatrix} =
\begin{vmatrix} 1,440 \\ 5,133 \\ -0,643 \\ 11,852 \\ 0,001\end{vmatrix}$