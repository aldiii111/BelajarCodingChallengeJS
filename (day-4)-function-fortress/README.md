# Apa yang Dipelajari di Day 4

Pada Day 4 ini, kamu belajar membuat aplikasi konversi suhu yang bisa mengubah Celsius ke Fahrenheit dan sebaliknya. Fokus pembelajaran adalah pembuatan fungsi dengan parameter dan return value untuk membuat kode lebih modular dan reusable.

## Konsep Utama yang Dipelajari

### 1. **Function dengan Parameter**
- Fungsi bisa menerima input (parameter) untuk diproses
- Parameter membuat fungsi lebih fleksibel dan reusable
```javascript
function celsiusToFahrenheit(temp) {
  return (temp * 9) / 5 + 32;
}
```

### 2. **Return Value**
- Fungsi bisa mengembalikan hasil dengan `return`
- Return value bisa disimpan di variabel atau langsung digunakan
```javascript
const result = celsiusToFahrenheit(25); // result = 77
```

### 3. **Function Composition**
- Memanggil fungsi dari dalam fungsi lain
- Memecah program kompleks jadi bagian-bagian kecil yang mudah dipahami
```javascript
function convertTemperature() {
  result = celsiusToFahrenheit(temp); // Panggil fungsi lain
}
```

### 4. **Conditional Logic dengan If-Else**
- Menggunakan if-else untuk memilih fungsi mana yang dipanggil
- Berdasarkan pilihan user dari dropdown
```javascript
if (type === "c-to-f") {
  result = celsiusToFahrenheit(temp);
} else if (type === "f-to-c") {
  result = fahrenheitToCelsius(temp);
}
```

### 5. **toFixed() untuk Format Angka**
- Membulatkan angka desimal ke jumlah digit tertentu
- Berguna untuk menampilkan hasil yang lebih rapi
```javascript
result.toFixed(2); // Tampilkan 2 digit desimal (misal: 77.00)
```

### 6. **Modular Programming**
- Memisahkan logic konversi ke fungsi terpisah
- Membuat kode lebih mudah di-maintain dan di-test
- Bisa digunakan ulang di tempat lain

## 💡 Poin Penting

- **Parameter** membuat fungsi fleksibel untuk berbagai input
- **Return value** membuat fungsi bisa memberikan output yang digunakan di tempat lain
- **Modular code** lebih mudah dibaca dan di-debug
- Validasi input tetap penting sebelum proses konversi

## 🌡️ Cara Kerja

1. User memasukkan angka suhu (misal: 25)
2. User pilih jenis konversi (C→F atau F→C)
3. Klik tombol "Konversi"
4. Program cek validasi input
5. Program panggil fungsi konversi yang sesuai
6. Fungsi hitung dan return hasil
7. Tampilkan hasil dengan format rapi (misal: "25°C = 77.00°F")

## 🔄 Formula Konversi

**Celsius ke Fahrenheit:**
```
F = (C × 9/5) + 32
```

**Fahrenheit ke Celsius:**
```
C = (F - 32) × 5/9
```

## 🚀 Konsep Baru

- **Function dengan parameter** - fungsi bisa terima input
- **Return value** - fungsi bisa kembalikan hasil
- **Function composition** - memanggil fungsi dari fungsi lain
- **toFixed()** - format angka desimal
- **Modular programming** - pisahkan logic jadi fungsi-fungsi kecil