# Apa yang Dipelajari di Day 2

Pada Day 2 ini, kamu belajar membuat kalkulator sederhana menggunakan JavaScript untuk memahami konsep dasar pemrograman web interaktif.

# Konsep Utama yang Dipelajari

### 1. **Variabel dan Seleksi Elemen DOM**

- Menggunakan `document.getElementById()` untuk mengambil elemen HTML
- Menyimpan elemen dalam variabel agar mudah digunakan

```javascript
const num1Input = document.getElementById("num1");
```

### 2. **Konversi Tipe Data**

- Menggunakan `parseFloat()` untuk mengubah input text menjadi angka
- Penting karena input HTML selalu berupa string

### 3. **Validasi Input**

- Menggunakan `isNaN()` untuk mengecek apakah input valid
- Mencegah error dengan pengecekan pembagian dengan nol

### 4. **Kontrol Flow**

- **Switch Statement**: Memilih operasi matematika berdasarkan pilihan user
- **If-Else**: Menangani kondisi error dan validasi

### 5. **Event Handling**

- `addEventListener()`: Menjalankan fungsi saat tombol diklik
- Membuat aplikasi menjadi interaktif dan responsif terhadap aksi user

### 6. **Manipulasi DOM**

- Menggunakan `textContent` untuk menampilkan hasil atau pesan error
- Mengubah konten halaman secara dinamis

## 💡 Poin Penting

- **Input validation** mencegah aplikasi crash
- **Event listener** membuat halaman interaktif tanpa reload
- **Switch statement** lebih rapi untuk multiple kondisi
- Selalu handle **edge cases** seperti pembagian dengan nol

## 🚀 Fitur Challenge (Opsional)

Tambahkan tombol **Reset** untuk mengosongkan semua input dan hasil!
