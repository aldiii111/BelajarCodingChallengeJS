# Apa yang dipelajari di Day 3

Pada Day 3 ini, kamu belajar membuat generator kata acak yang menghasilkan kombinasi huruf random sesuai panjang yang diinginkan. Fokus pembelajaran adalah manipulasi string dan penggunaan angka random.

# Konsep Utama yang dipelajari

### 1. **String sebagai Array**
- String bisa diakses seperti array dengan index
- Menggunakan `slice()` untuk mengambil karakter tertentu
```javascript
const alphabet = "abcdefghijklmnopqrstuvwxyz";
const huruf = alphabet.slice(0, 1); // Ambil huruf 'a'
```

### 2. **Math.random() dan Math.floor()**
- `Math.random()`: Menghasilkan angka acak antara 0 sampai 1
- `Math.floor()`: Membulatkan ke bawah untuk mendapat index integer
```javascript
const randomIndex = Math.floor(Math.random() * alphabet.length);
```

### 3. **Looping**
- Menggunakan **for loop** untuk mengulang proses
- Loop sebanyak panjang kata yang diinginkan
- Setiap iterasi menambahkan 1 huruf random

### 4. **String Concatenation**
- `concat()`: Menggabungkan string dengan string lain
- Membangun kata secara bertahap dari string kosong
```javascript
word = word.concat(randomLetter);
```

### 5. **parseInt() untuk Konversi**
- Mengubah input text menjadi angka integer
- Berbeda dengan `parseFloat()` karena hanya butuh angka bulat

### 6. **Template Literal**
- Menggunakan backtick `` ` `` dan `${}` untuk menampilkan variabel
```javascript
outputDiv.textContent = `Kata Acak: ${word}`;
```

## 💡 Poin Penting

- **Math.random()** selalu menghasilkan hasil berbeda setiap kali dipanggil
- **Slice()** mengambil bagian string tanpa mengubah string asli
- **Loop** sangat berguna untuk tugas berulang
- Validasi input penting untuk mencegah error (panjang minimal 1)

## 🎲 Cara Kerja

1. User memasukkan angka (misal: 5)
2. Program loop sebanyak 5 kali
3. Setiap loop: pilih huruf random dari alphabet
4. Gabungkan semua huruf jadi satu kata
5. Tampilkan hasil (misal: "kbxqm")

## 🚀 Konsep Baru

- **String manipulation** dengan slice dan concat
- **Random number generation** untuk hasil tidak terprediksi
- **Loop** untuk proses berulang
- **Template literal** untuk output lebih rapi