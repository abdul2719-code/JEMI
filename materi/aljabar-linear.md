# 📐 Aljabar Linear untuk Pendidikan Matematika

## 🎯 Kompetensi Dasar
**Siswa mampu memahami dan menerapkan**:
1. Konsep vektor dalam ruang 2D dan 3D
2. Operasi dasar vektor (penjumlahan, perkalian skalar, dot product)
3. Matriks sebagai representasi transformasi linear
4. Aplikasi dalam masalah kontekstual

## 📖 Materi Inti

### A. KONSEP VEKTOR
#### 1. Pengertian Vektor
**Definisi**: Besaran yang memiliki magnitude (besar) dan arah

**Notasi**:
\[
\vec{v} = \begin{bmatrix} x \\ y \end{bmatrix} \quad \text{atau} \quad \vec{v} = x\hat{i} + y\hat{j}
\]

**Contoh dalam kehidupan**:
- Kecepatan mobil: 60 km/jam ke utara
- Gaya gravitasi: 9.8 m/s² ke bawah
- Perpindahan: 5 meter ke timur

#### 2. Operasi Vektor Dasar
**Penjumlahan Vektor** (Aturan Jajaran Genjang):
\[
\vec{a} + \vec{b} = \begin{bmatrix} a_x + b_x \\ a_y + b_y \end{bmatrix}
\]

**Perkalian Skalar**:
\[
k\vec{v} = \begin{bmatrix} kx \\ ky \end{bmatrix}, \quad k \in \mathbb{R}
\]

**Dot Product** (Perkalian Titik):
\[
\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y = |\vec{a}||\vec{b}|\cos\theta
\]

### B. MATRIKS DAN TRANSFORMASI
#### 1. Pengertian Matriks
\[
A = \begin{bmatrix}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{bmatrix}_{2\times2}
\]

**Matriks Identitas**:
\[
I = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}
\]

**Matriks Rotasi** (sudut θ):
\[
R(\theta) = \begin{bmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{bmatrix}
\]

#### 2. Transformasi Linear
**Translasi** (Pergeseran):
\[
T(\vec{v}) : \begin{bmatrix} x' \\ y' \end{bmatrix} = \begin{bmatrix} x \\ y \end{bmatrix} + \begin{bmatrix} a \\ b \end{bmatrix}
\]

**Rotasi** (Perputaran):
\[
R(\theta) : \begin{bmatrix} x' \\ y' \end{bmatrix} = \begin{bmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix}
\]

## 🎮 Aktivitas Pembelajaran

### Level 1: Pemahaman Konsep
**Aktivitas**: "Vector Treasure Hunt"
- Siswa membuat peta dengan koordinat
- Setiap lokasi memiliki vektor perpindahan
- Mencari harta karun dengan operasi vektor

### Level 2: Aplikasi
**Aktivitas**: "Physics in Sports"
- Analisis vektor kecepatan dalam olahraga
- Video analysis menggunakan tracker
- Hitung resultan gaya

### Level 3: Kreatif
**Proyek**: "Mathematical Art"
- Buat karya seni dengan transformasi matriks
- Gunakan rotasi, refleksi, scaling
- Presentasi proses matematis

## 🛠️ Tools Pendukung

### GeoGebra
```geogebra
# Visualisasi vektor
v = Vector((3, 2))
w = Vector((-1, 4))
v + w

# Transformasi matriks
A = {{2, 1}, {-1, 3}}
ApplyMatrix(A, (1, 2))
import numpy as np
import matplotlib.pyplot as plt

# Operasi vektor
v = np.array([3, 2])
w = np.array([-1, 4])
print("v + w =", v + w)
print("Dot product =", np.dot(v, w))

# Visualisasi
plt.quiver(0, 0, v[0], v[1], angles='xy', scale_units='xy', scale=1, color='r')
plt.quiver(0, 0, w[0], w[1], angles='xy', scale_units='xy', scale=1, color='b')
plt.xlim(-2, 5)
plt.ylim(-1, 5)
plt.grid()
plt.show()
