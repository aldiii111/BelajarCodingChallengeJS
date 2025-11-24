# Apa yang Dipelajari di Day 5

Pada Day 5 ini, kamu belajar membuat aplikasi quiz sederhana dengan sistem scoring. User menjawab pertanyaan dengan memilih "Ya" atau "Tidak", kemudian sistem akan menghitung skor berdasarkan jawaban yang benar. Fokus pembelajaran adalah boolean logic, conditional statements, dan counter variables.

# Konsep Utama yang Dipelajari

### 1. **Boolean Logic**
- Nilai boolean hanya ada 2: `true` atau `false`
- Digunakan untuk membuat keputusan dalam program
- Conditional statements bergantung pada boolean
```javascript
if (selectedAnswer) {  // true jika ada jawaban
  // Jalankan kode ini
}
```

### 2. **Truthy dan Falsy Values**
- **Truthy**: Nilai yang dianggap `true` dalam konteks boolean
- **Falsy**: `null`, `undefined`, `0`, `""`, `false`, `NaN`
- `selectedAnswer` akan `null` (falsy) jika tidak ada yang dipilih
```javascript
const selectedAnswer = document.querySelector('input[name="answer"]:checked');
// Jika tidak ada yang dipilih → null (falsy)
// Jika ada yang dipilih → element object (truthy)
```

### 3. **querySelector dengan :checked**
- `querySelector()`: Mencari elemen dengan CSS selector
- `:checked`: Pseudo-class untuk radio/checkbox yang dipilih
- `name="answer"`: Memilih dari group radio button tertentu
```javascript
const selectedAnswer = document.querySelector('input[name="answer"]:checked');
```

### 4. **Counter Variable**
- Variabel untuk menghitung/menyimpan angka yang berubah
- Menggunakan `let` karena nilai bisa berubah (mutable)
- Increment dengan operator `+=` untuk menambah nilai
```javascript
let score = 0;  // Inisialisasi
score += 1;     // Tambah 1 (sama dengan: score = score + 1)
```

### 5. **Nested If-Else**
- If-else di dalam if-else lain
- Level pertama: cek apakah ada jawaban
- Level kedua: cek jawaban benar atau salah
```javascript
if (selectedAnswer) {           // Level 1: Ada jawaban?
  if (answerValue === "ya") {   // Level 2: Jawaban benar?
    score += 1;
  } else {
    // Jawaban salah
  }
} else {
  // Tidak ada jawaban
}
```

### 6. **Comparison Operator (===)**
- `===`: Strict equality - cek tipe data DAN nilai
- Lebih aman daripada `==` yang bisa mengkonversi tipe
```javascript
if (answerValue === "ya") {  // Cek apakah string "ya"
  // Benar
}
```

## 💡 Poin Penting

- **Boolean** adalah dasar dari semua decision-making dalam programming
- **Truthy/Falsy** memudahkan pengecekan tanpa perlu `=== null`
- **querySelector** lebih fleksibel karena bisa pakai CSS selector
- **Counter** sangat berguna untuk tracking score, likes, votes, dll
- **Nested if-else** untuk kondisi yang lebih kompleks
- Selalu gunakan `===` untuk comparison, bukan `==`

## 🎮 Cara Kerja

1. User melihat pertanyaan
2. User pilih jawaban "Ya" atau "Tidak" (radio button)
3. User klik tombol "Submit Jawaban"
4. Program cek apakah ada jawaban yang dipilih
   - Jika tidak ada → tampilkan error
   - Jika ada → lanjut ke step 5
5. Program cek value jawaban
   - Jika "ya" → score +1, tampilkan "Benar!"
   - Jika "tidak" → score tetap, tampilkan "Salah!"
6. Tampilkan skor terkini

## 📊 Sistem Scoring

- **Jawaban "Ya"** → Skor +1 (benar)
- **Jawaban "Tidak"** → Skor +0 (salah)
- **Tidak menjawab** → Error message

## 🚀 Konsep Baru

- **Boolean logic** untuk decision making
- **Truthy/Falsy values** untuk pengecekan simpel
- **querySelector** dengan CSS selector (lebih powerful dari getElementById)
- **Radio button** untuk pilihan ekslusif
- **Counter variable** dengan `let` untuk nilai yang berubah
- **Nested if-else** untuk kondisi bertingkat
- **Comparison operator** `===` untuk strict equality
