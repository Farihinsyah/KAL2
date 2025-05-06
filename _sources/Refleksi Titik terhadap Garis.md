---
title: Refleksi Titik terhadap Garis

---

# Penjelasan Refleksi Titik terhadap Garis \( y = 2 \)

Dalam transformasi geometri, refleksi titik terhadap suatu garis dapat dilakukan menggunakan matriks dan translasi. Pada kasus ini, kita akan merefleksikan titik terhadap garis horizontal \( y = 2 \). Berikut adalah penjelasan langkah-langkah yang diambil dalam proses refleksi tersebut.

## Langkah 1: Matriks Refleksi terhadap Sumbu-X

Untuk refleksi terhadap garis horizontal \( y = 2 \), kita perlu menggunakan dua operasi dasar:

1. **Refleksi terhadap sumbu-X:** 
   Matriks refleksi terhadap sumbu-X membalikkan koordinat \( y \) dari titik yang diberikan. Matriks refleksi terhadap sumbu-X adalah:

   $$
   B = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}
   $$

   Matriks ini membalikkan koordinat \( y \), tetapi tidak mengubah \( x \).

## Langkah 2: Translasi untuk Menyesuaikan dengan Garis \( y = 2 \)

Setelah refleksi terhadap sumbu-X, kita perlu melakukan **translasi** agar titik hasil refleksi berada pada posisi yang benar relatif terhadap garis \( y = 2 \). Garis \( y = 2 \) berada pada jarak 2 satuan di atas sumbu-X. Oleh karena itu, kita perlu menambahkan vektor translasi yang menggeser hasil refleksi ke posisi yang tepat.

Vektor translasi yang digunakan adalah:

$$
t = \begin{bmatrix} 0 \\ 4 \end{bmatrix}
$$

Vektor ini menggeser titik hasil refleksi sebesar 4 satuan di atas sumbu-X untuk mencapai garis \( y = 2 \).

## Langkah 3: Menghitung Titik Refleksi

Titik asal yang akan direfleksikan adalah \( (x, y) = (1, 1) \). Proses refleksi dilakukan dengan matriks transformasi yang terdiri dari refleksi dan translasi:

$$
B_{\text{trans}} = B \cdot \begin{bmatrix} x \\ y \end{bmatrix} + t
$$

Substitusi koordinat \( (x, y) = (1, 1) \) ke dalam persamaan ini menghasilkan:

$$
B_{\text{trans}} = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 1 \end{bmatrix} + \begin{bmatrix} 0 \\ 4 \end{bmatrix} = \begin{bmatrix} 1 \\ -1 \end{bmatrix} + \begin{bmatrix} 0 \\ 4 \end{bmatrix} = \begin{bmatrix} 1 \\ 3 \end{bmatrix}
$$

Dengan demikian, titik hasil refleksi adalah \( (1, 3) \).

## Langkah 4: Visualisasi Grafik

Untuk memvisualisasikan refleksi ini, kita menggambar titik asal dan titik hasil refleksi pada grafik. Titik asal diberi tanda merah (ro), dan titik hasil refleksi diberi tanda biru (bo). Garis \( y = 2 \) juga digambarkan sebagai garis hijau.

### Grafik:

1. **Titik asal:** Titik \( (1, 1) \) digambarkan dengan tanda merah.
2. **Titik hasil refleksi:** Titik \( (1, 3) \) digambarkan dengan tanda biru.
3. **Garis \( y = 2 \):** Garis hitam sebagai garis refleksi.
4. **Garis horizontal:** Untuk menunjukkan sumbu X dan Y yang digunakan sebagai referensi.

koordinats = np.array([[1], [1]])
x = koordinats[0,:]
y = koordinats[1,:]

B = np.array([[1,0],[0,-1]])
t = np.array([[0],[4]])
B_trans = B @ koordinats + t

x_LT2 = B_trans[0,:]
y_LT2 = B_trans[1,:]

fig, ax = plt.subplots()
ax.plot(x,y,'ro')
ax.plot(x_LT2,y_LT2,'bo')
ax.plot(x,y,'r',ls="--")
ax.plot(x_LT2,y_LT2,'b')
ax.axhline(y=2,color="black",ls=":",label="y=2")
ax.axvline(x=0,color="k",ls=":")
ax.axhline(y=0,color="k",ls=":")
ax.grid(True)
ax.axis([0,4,0,4])
ax.set_aspect('equal')
ax.set_title("Refleksi sumbu Y = 2")

![image](https://hackmd.io/_uploads/HkuxZePgge.png)

---

# Penjelasan Refleksi Titik terhadap Garis \( x = 2 \)

Dalam transformasi geometri, refleksi titik terhadap suatu garis dapat dilakukan dengan menggunakan matriks refleksi dan translasi. Pada kasus ini, kita akan merefleksikan titik terhadap garis vertikal \( x = 2 \). Berikut adalah penjelasan langkah-langkah yang diambil dalam proses refleksi tersebut.

## Langkah 1: Matriks Refleksi terhadap Sumbu-Y

Untuk refleksi terhadap garis vertikal \( x = 2 \), kita perlu menggunakan dua operasi dasar:

1. **Refleksi terhadap sumbu-Y:**
   Matriks refleksi terhadap sumbu-Y membalikkan koordinat \( x \) dari titik yang diberikan. Matriks refleksi terhadap sumbu-Y adalah:

   $$
   B = \begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}
   $$

   Matriks ini membalikkan koordinat \( x \), tetapi tidak mengubah \( y \).

## Langkah 2: Translasi untuk Menyesuaikan dengan Garis \( x = 2 \)

Setelah refleksi terhadap sumbu-Y, kita perlu melakukan **translasi** agar titik hasil refleksi berada pada posisi yang benar relatif terhadap garis \( x = 2 \). Garis \( x = 2 \) berada pada jarak 2 satuan di sebelah kanan sumbu-Y. Oleh karena itu, kita perlu menambahkan vektor translasi yang menggeser hasil refleksi ke posisi yang tepat.

Vektor translasi yang digunakan adalah:

$$
t = \begin{bmatrix} 4 \\ 0 \end{bmatrix}
$$

Vektor ini menggeser titik hasil refleksi sebesar 4 satuan ke kanan sumbu-Y untuk mencapai garis \( x = 2 \).

## Langkah 3: Menghitung Titik Refleksi

Titik asal yang akan direfleksikan adalah \( (x, y) = (1, 1) \). Proses refleksi dilakukan dengan matriks transformasi yang terdiri dari refleksi dan translasi:

$$
B_{\text{trans}} = B \cdot \begin{bmatrix} x \\ y \end{bmatrix} + t
$$

Substitusi koordinat \( (x, y) = (1, 1) \) ke dalam persamaan ini menghasilkan:

$$
B_{\text{trans}} = \begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 1 \end{bmatrix} + \begin{bmatrix} 4 \\ 0 \end{bmatrix} = \begin{bmatrix} -1 \\ 1 \end{bmatrix} + \begin{bmatrix} 4 \\ 0 \end{bmatrix} = \begin{bmatrix} 3 \\ 1 \end{bmatrix}
$$

Dengan demikian, titik hasil refleksi adalah \( (3, 1) \).

## Langkah 4: Visualisasi Grafik

Untuk memvisualisasikan refleksi ini, kita menggambar titik asal dan titik hasil refleksi pada grafik. Titik asal diberi tanda merah (ro), dan titik hasil refleksi diberi tanda biru (bo). Garis \( x = 2 \) juga digambarkan sebagai garis hitam.

### Grafik:

1. **Titik asal:** Titik \( (1, 1) \) digambarkan dengan tanda merah.
2. **Titik hasil refleksi:** Titik \( (3, 1) \) digambarkan dengan tanda biru.
3. **Garis \( x = 2 \):** Garis hitam sebagai garis refleksi.
4. **Garis sumbu X dan Y:** Untuk menunjukkan sumbu referensi.

koordinats = np.array([[1], [1]])
x = koordinats[0,:]
y = koordinats[1,:]

B = np.array([[-1,0],[0,1]])
t = np.array([[4],[0]])
B_trans = B @ koordinats + t

x_LT2 = B_trans[0,:]
y_LT2 = B_trans[1,:]

fig, ax = plt.subplots()
ax.plot(x,y,'ro')
ax.plot(x_LT2,y_LT2,'bo')
ax.plot(x,y,'r',ls="--")
ax.plot(x_LT2,y_LT2,'b')
ax.axvline(x=2,color="black",ls=":",label="x=2")
ax.axvline(x=0,color="k",ls=":")
ax.axhline(y=0,color="k",ls=":")
ax.grid(True)
ax.axis([0,4,0,4])
ax.set_aspect('equal')
ax.set_title("Refleksi sumbu X = 2")


![image](https://hackmd.io/_uploads/HJ_QWxveel.png)

---

# Penjelasan Refleksi Titik terhadap Garis \( y = x \)

Refleksi titik terhadap garis \( y = x \) adalah transformasi geometri di mana titik asal dipindahkan sehingga posisinya simetris terhadap garis tersebut. Untuk memahami proses ini, mari kita lihat langkah-langkah berikut.

## Langkah 1: Matriks Refleksi terhadap Garis \( y = x \)

Refleksi terhadap garis \( y = x \) dapat dilakukan dengan menggunakan matriks transformasi. Matriks refleksi untuk garis \( y = x \) dapat dinyatakan sebagai:

$$
B = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}
$$

Matriks ini bertukar posisi komponen \( x \) dan \( y \) dari titik yang diberikan. Jadi, setelah diterapkan, koordinat titik \( (x, y) \) akan menjadi \( (y, x) \).

## Langkah 2: Menghitung Titik Refleksi

Titik asal yang akan direfleksikan adalah \( (x, y) = (1, 2) \). Proses refleksi dilakukan dengan mengalikan matriks refleksi \( B \) dengan vektor koordinat asal \( (x, y) \):

$$
B_{\text{trans}} = B \cdot \begin{bmatrix} x \\ y \end{bmatrix}
$$

Substitusi koordinat \( (x, y) = (1, 2) \) ke dalam persamaan ini menghasilkan:

$$
B_{\text{trans}} = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 2 \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
$$

Dengan demikian, titik hasil refleksi adalah \( (2, 1) \).

## Langkah 3: Visualisasi Grafik

Untuk memvisualisasikan refleksi ini, kita menggambar titik asal dan titik hasil refleksi pada grafik. Titik asal diberi tanda merah (ro), dan titik hasil refleksi diberi tanda biru (bo). Garis \( y = x \) digambarkan sebagai garis hitam.

### Grafik:

1. **Titik asal:** Titik \( (1, 2) \) digambarkan dengan tanda merah.
2. **Titik hasil refleksi:** Titik \( (2, 1) \) digambarkan dengan tanda biru.
3. **Garis \( y = x \):** Garis hitam sebagai garis refleksi.
4. **Garis sumbu X dan Y:** Untuk menunjukkan sumbu referensi.

koordinats = np.array([[1], [2]])
x = koordinats[0,:]
y = koordinats[1,:]

B = np.array([[0,1],[1,0]])
B_trans = B @ koordinats

x_LT2 = B_trans[0,:]
y_LT2 = B_trans[1,:]

fig, ax = plt.subplots()
ax.plot(x,y,'ro')
ax.plot(x_LT2,y_LT2,'bo')
ax.plot(x,y,'r',ls="--")
ax.plot(x_LT2,y_LT2,'b')
ax.plot([0,4],[0,4],'black',ls=":",label="y=x")
ax.axvline(x=0,color="k",ls=":")
ax.axhline(y=0,color="k",ls=":")
ax.grid(True)
ax.axis([0,4,0,4])
ax.set_aspect('equal')
ax.set_title("Refleksi terhadap garis y = x")


![image](https://hackmd.io/_uploads/BkDEWePgxg.png)

