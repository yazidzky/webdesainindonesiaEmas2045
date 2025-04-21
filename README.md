# webdesainindonesiaEmas2045

## 📌 Pengertian dan Tujuan Kode

Kode ini merupakan skrip JavaScript dan CSS untuk sebuah website interaktif bertema *Indonesia Emas 2045*. Website ini dirancang untuk menyampaikan visi pembangunan Indonesia melalui animasi, navigasi dinamis, dan konten visual yang menarik. Tujuannya adalah untuk menyajikan informasi secara engaging lewat fitur splash screen, navigasi flip card, peta interaktif, mode terang/gelap, komentar pengguna, dan terjemahan bahasa.

---

## 🔍 Penjelasan Tiap Bagian Kode

### `Splash Screen`
```javascript
window.addEventListener('load', () => {
  setTimeout(() => {
    document.getElementById('splash-screen').style.display = 'none';
    document.getElementById('main-content').style.display = 'block';
    document.getElementById('navbar').style.opacity = 1;
    document.getElementById('navbar').style.transition = 'opacity 1s';
  }, 5000);
});
```
📌 Menampilkan layar pembuka selama 5 detik sebelum konten utama dimunculkan.

---

### `Navigasi Interaktif & Responsif`
```javascript
function toggleMenu() {
  const menu = document.getElementById('navbarMenu');
  menu.classList.toggle('active');
}
```
📌 Menampilkan atau menyembunyikan menu navigasi, berguna untuk tampilan mobile.

---

### `Navigasi Pilar dan Flip Card`
```javascript
function showPillar(direction) { ... }
function showDirectionCard(direction) { ... }
function updateTargets(indexChange) { ... }
```
📌 Fungsi-fungsi ini mengatur tampilan kartu informasi secara dinamis berdasarkan arah navigasi (next/prev). Terdapat adaptasi untuk tampilan desktop dan mobile.

---

### `Interaksi Peta`
```javascript
document.querySelectorAll('.map-btn').forEach(button => { ... });
```
📌 Menampilkan deskripsi singkat dan lengkap berdasarkan tombol destinasi yang ditekan. Juga mengubah gambar latar belakang peta dan highlight tombol aktif.

---

### `Mode Gelap / Terang`
```javascript
themeToggleIcon.addEventListener('click', () => {
  document.body.classList.toggle('dark-mode');
  ...
});
```
📌 Menyediakan saklar antara tampilan terang dan gelap, meningkatkan aksesibilitas dan kenyamanan pengguna.

---

### `Komentar dan Terjemahan`
```javascript
commentIcon.addEventListener('click', () => {
  ...
});
translateIcon.addEventListener('click', () => {
  ...
});
```
📌 Pengguna dapat memberikan komentar atau mengganti bahasa tampilan (Indonesia, Inggris, Jepang) untuk memahami konten dalam bahasa pilihan mereka.

---

## 🎲 Analogi Sederhana Algoritma

Bayangkan website ini seperti sebuah pameran virtual. Ketika kamu masuk:
- Kamu disambut oleh pintu gerbang (splash screen).
- Setelah masuk, kamu bisa berjalan ke berbagai ruangan (pilar) dan membaca informasi di papan informasi yang bisa dibalik (flip card).
- Ada denah (map) yang bisa kamu klik untuk tahu detail tiap ruangan.
- Kamu bisa menyalakan atau mematikan lampu pameran (dark mode).
- Ada buku tamu (komentar) dan pemandu multibahasa (translator).

Semua bagian itu berjalan otomatis tergantung interaksi kamu—seolah-olah kamu mengunjungi pameran futuristik yang responsif.

---

## ✅ Kesimpulan

Kode ini membentuk sebuah website presentasi interaktif dengan pengalaman pengguna yang dinamis, responsif, dan ramah bagi berbagai perangkat dan bahasa. Fungsionalitas seperti splash screen, navigasi interaktif, dark mode, serta fitur komentar dan terjemahan menjadikan situs ini modern, edukatif, dan menarik. Sangat cocok untuk kampanye edukasi, presentasi rencana pembangunan, atau media informasi digital skala nasional.
