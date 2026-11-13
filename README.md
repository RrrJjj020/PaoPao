<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Birthday Surprise ❤️</title>
<style>
:root{--navy:#111d32;--blue:#438df2;--cream:#fff9f1;--white:#f8fbff}
*{box-sizing:border-box}
body{margin:0;min-height:100vh;font-family:Arial,Helvetica,sans-serif;background:var(--cream);color:#fff}
.screen{min-height:100vh;display:flex;align-items:center;justify-content:center;padding:18px}
.login-screen{background:radial-gradient(circle at 8% 12%,#477a9e 0,transparent 25%),radial-gradient(circle at 95% 90%,#397bb7 0,transparent 28%),linear-gradient(120deg,#14213b,#1b2b4d);position:relative;overflow:hidden}
.login-card{width:min(410px,92vw);min-height:420px;padding:46px 28px 34px;border:1px solid rgba(255,255,255,.07);border-radius:27px;background:rgba(8,19,38,.52);box-shadow:0 22px 65px rgba(0,0,0,.2);text-align:center;position:relative}
.heart{font-size:54px;line-height:1.1;margin:0 0 25px;color:#fff;text-shadow:0 2px 8px #fff7}
h1{font-size:30px;margin:0 0 8px;font-weight:800;letter-spacing:-.7px}
.heart-small{font-size:27px;margin:0 0 8px}
.subtitle{color:#dce6f5;margin:0 0 31px;font-size:16px}
input{width:100%;border:0;border-radius:19px;padding:17px 16px;font-size:16px;background:#f1f1f3;color:#26344a;outline:none;margin-bottom:14px}
input::placeholder{color:#87909d}
button{border:0;border-radius:17px;padding:16px 20px;background:linear-gradient(100deg,#5ca5ff,#367ee9);color:white;font-size:16px;font-weight:700;cursor:pointer;box-shadow:0 9px 24px #2f82ee45}
button:hover{filter:brightness(1.08);transform:translateY(-1px)}
.login-btn{width:100%}
.error{min-height:20px;color:#ffb9c3;font-size:13px;margin-top:12px}
.decoration{position:absolute;font-size:65px;right:-8px;bottom:4px;opacity:.9;transform:rotate(-13deg);pointer-events:none}
.hidden{display:none!important}
.content-screen{min-height:100vh;background:radial-gradient(circle at top right,#345f91,transparent 36%),linear-gradient(145deg,#111d32,#1e3458);padding:28px 16px 60px}
.site{max-width:980px;margin:auto}
.topline{text-align:center;color:#c8d9f0;font-size:14px;letter-spacing:2px;text-transform:uppercase}
.hero{text-align:center;padding:44px 10px 28px}
.hero .big{font-size:64px;margin:0 0 12px}
.hero h2{font-size:clamp(32px,6vw,54px);margin:0 0 12px}
.hero p{color:#d9e5f5;font-size:17px;line-height:1.6}
.nav{display:flex;flex-wrap:wrap;gap:9px;justify-content:center;margin:22px 0 28px}
.nav button{padding:11px 15px;font-size:13px;border-radius:999px;background:#ffffff18;border:1px solid #ffffff2c;box-shadow:none}
.nav button.active{background:#438df2}
.panel{background:#ffffff10;border:1px solid #ffffff20;border-radius:24px;padding:28px;box-shadow:0 18px 45px #0002;min-height:260px}
.panel h3{text-align:center;font-size:28px;margin:0 0 16px}
.panel p{color:#e2eaf6;line-height:1.8;text-align:center}
.photo-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:20px}
.photo{aspect-ratio:1/1;border:1px dashed #d5e5ff88;border-radius:16px;display:flex;align-items:center;justify-content:center;text-align:center;padding:12px;color:#d5e5ff;background:#ffffff09;font-size:13px}
.letter{max-width:650px;margin:auto;background:#fff9f0;color:#34415a;border-radius:18px;padding:26px;line-height:1.9;white-space:pre-line}
.footer{text-align:center;color:#b9cbe2;margin-top:26px;font-size:13px}
@media(max-width:560px){.login-card{min-height:400px;padding:40px 22px 30px}.login-card h1{font-size:27px}.photo-grid{grid-template-columns:repeat(2,1fr)}.panel{padding:22px 16px}}
</style>
</head>
<body>
<section id="login" class="screen login-screen">
  <div class="login-card">
    <div class="heart">♡</div>
    <h1>Masukan Password</h1>
    <div class="heart-small">💖</div>
    <p class="subtitle">a little surprise for you</p>
    <form id="loginForm">
      <input id="password" type="password" placeholder="Masukan password..." autocomplete="off" aria-label="Password">
      <button class="login-btn" type="submit">Masuk</button>
      <div id="error" class="error"></div>
    </form>
    <div class="decoration">♡</div>
  </div>
</section>

<main id="birthday" class="content-screen hidden">
 <div class="site">
  <div class="topline">made with love, just for you</div>
  <header class="hero">
    <div class="big">🎂</div>
    <h2>Happy Birthday, Sayang!</h2>
    <p>Hari ini adalah hari spesial seseorang yang sangat berarti.<br>Aku punya beberapa kejutan kecil untukmu. ❤️</p>
  </header>
  <nav class="nav" aria-label="Menu kejutan">
    <button class="active" data-page="welcome">Birthday Surprise</button>
    <button data-page="memories">Our Memories</button>
    <button data-page="letter">Love Letter</button>
    <button data-page="wishes">Birthday Wishes</button>
    <button data-page="final">Final Surprise</button>
  </nav>
  <section id="welcome" class="panel page">
    <h3>♡ For My Favorite Person ♡</h3>
    <p>Selamat ulang tahun, cintaku. Terima kasih sudah hadir dan membuat hari-hariku lebih berwarna. Semoga halaman kecil ini bisa membuatmu tersenyum, seperti kamu yang selalu punya cara untuk membuatku bahagia.</p>
    <p>Jelajahi setiap bagian ya. Ada sesuatu yang aku siapkan khusus untukmu. 💗</p>
  </section>
  <section id="memories" class="panel page hidden">
    <h3>Our Memories 📸</h3>
    <p>Ganti kotak-kotak ini dengan foto-foto terbaik kalian.</p>
    <div class="photo-grid">
      <div class="photo">Tambahkan foto pertama</div><div class="photo">Tambahkan foto kedua</div><div class="photo">Tambahkan foto ketiga</div>
      <div class="photo">Tambahkan foto keempat</div><div class="photo">Tambahkan foto kelima</div><div class="photo">Tambahkan foto keenam</div>
    </div>
  </section>
  <section id="letter" class="panel page hidden">
    <h3>A Letter For You 💌</h3>
    <div class="letter">Untuk seseorang yang paling istimewa,

Selamat ulang tahun, sayang. Aku mungkin tidak selalu pandai mengungkapkan perasaan, tetapi aku ingin kamu tahu betapa berharganya dirimu untukku.

Terima kasih untuk setiap tawa, cerita, perhatian, dan kenangan yang kita buat bersama. Aku berharap tahun ini membawa banyak kebahagiaan, kesehatan, dan semua hal baik yang kamu impikan.

Aku akan terus mendukungmu dan berharap bisa membuat lebih banyak kenangan indah bersamamu.

With love,
Your favorite person ❤️</div>
  </section>
  <section id="wishes" class="panel page hidden">
    <h3>My Wishes For You ✨</h3>
    <p>Semoga kamu selalu sehat, bahagia, dimudahkan dalam setiap langkah, dikelilingi orang-orang yang menyayangimu, dan satu per satu impianmu menjadi nyata.</p>
    <p>Jangan pernah lupa bahwa kamu pantas mendapatkan hal-hal baik di dunia ini. ❤️</p>
  </section>
  <section id="final" class="panel page hidden">
    <h3>One Last Thing… 💝</h3>
    <p>Di antara banyak hal baik yang terjadi dalam hidupku, mengenalmu adalah salah satu yang paling aku syukuri.</p>
    <p><strong>Happy birthday, my love. I love you! ❤️</strong></p>
    <p>🎈 🎂 💐 🎁</p>
  </section>
  <div class="footer">A little website, with a lot of love. ♡</div>
 </div>
</main>
<script>
/*
  PENTING: Ganti tanggal di bawah dengan tanggal lahir pacarmu.
  Format wajib YYYY-MM-DD. Contoh: 2000-08-17
  Password yang diketik di halaman depan: DD-MM-YYYY
*/
const BIRTHDAY_DATE = "YYYY-MM-DD";

document.getElementById("loginForm").addEventListener("submit", function(e){
  e.preventDefault();
  const entered = document.getElementById("password").value.trim();
  const expected = BIRTHDAY_DATE === "YYYY-MM-DD" ? "" : BIRTHDAY_DATE.split("-").reverse().join("-");
  if (!expected) {
    document.getElementById("error").textContent = "Atur tanggal lahir di bagian BIRTHDAY_DATE pada kode terlebih dahulu.";
    return;
  }
  if (entered === expected) {
    document.getElementById("login").classList.add("hidden");
    document.getElementById("birthday").classList.remove("hidden");
    window.scrollTo(0,0);
  } else {
    document.getElementById("error").textContent = "Password belum tepat. Coba lagi ya ❤️";
  }
});
document.querySelectorAll(".nav button").forEach(btn=>{
  btn.addEventListener("click",()=>{
    document.querySelectorAll(".nav button").forEach(b=>b.classList.remove("active"));
    document.querySelectorAll(".page").forEach(p=>p.classList.add("hidden"));
    btn.classList.add("active");
    document.getElementById(btn.dataset.page).classList.remove("hidden");
  });
});
</script>
</body>
</html>
