<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Simalem Convention Hall</title>

<!-- Swiper -->
<link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css"/>

<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600;700;900&family=Montserrat:wght@400;500;600;700&display=swap" rel="stylesheet">

<!-- Font Awesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<!-- CSS -->
<link rel="stylesheet" href="style.css">
</head>

<body>

<header id="header">
    <div class="logo"><img src="LOGO.png"></div>

    <nav id="nav">
        <a href="#home">HOME</a>
        <a href="#about">ABOUT</a>
        <a href="#fasilitas">FASILITAS</a>
        <a href="#gallery">GALLERY</a>
        <a href="#contact">CONTACT</a>
        <input type="text" class="search-box" placeholder="Cari...">
    </nav>

    <div class="header-controls">
        <i class="fas fa-search icon-small" id="searchIcon"></i>
        <div class="mobile-menu-icon" id="mobileMenu">
            <i class="fas fa-bars"></i>
        </div>
    </div>
</header>

<!-- HOME -->
<section id="home">
    <div class="swiper-container">
        <div class="swiper-wrapper">
            <div class="swiper-slide">
                <video src="JAMBUR SIMALAM.mp4" autoplay muted loop playsinline></video>
            </div>
        </div>
    </div>
</section>

<!-- ABOUT -->
<section id="about" class="container about-section">
<h1>Tentang <span class="brand-font">Simalem Convention Hall</span></h1>

<p>
<span class="brand-font">Simalem Convention Hall</span> adalah gedung pertemuan megah di Cibinong yang dapat digunakan untuk wedding, wisuda, acara keagamaan, rapat, ulang tahun, dan berbagai acara lainnya. Gedung 2 lantai ini memiliki kapasitas hingga 1.200 orang, full AC, serta dirancang untuk kenyamanan tamu dan penyelenggara acara.
</p>

<p>
Fasilitas yang tersedia meliputi 2 ruang rias, 1 ruang ganti, toilet di setiap sudut gedung baik lantai atas maupun bawah, serta toilet di masing-masing ruang rias. Tersedia juga mushola, ruang rapat khusus, pantry untuk catering, dan area parkir luas dengan kapasitas hingga 350 mobil
</p>

<p>
Selain gedung utama, tersedia venue khusus untuk acara <em>intimate</em> dengan kapasitas 200 orang, full AC, dan dilengkapi toilet di dalam ruangan.
</p>
</section>

<!-- FASILITAS -->
<section id="fasilitas" class="container">
<h1>Fasilitas Unggulan</h1>

<div class="facility-group">
<h2>Wedding Hall</h2>
<div class="facility-images">
<img src="wedding hall.webp">
<img src="gedung (8).jpg">
<img src="gedung (9).jpg">
<img src="gedung (6).jpg">
</div>

<h2>Wedding Hall</h2>
<div class="facility-images">
<img src="wedding hall.webp">
<img src="gedung (8).jpg">
<img src="gedung (9).jpg">
<img src="gedung (6).jpg">
</div>

<h2>Wedding Hall</h2>
<div class="facility-images">
<img src="wedding hall.webp">
<img src="gedung (8).jpg">
<img src="gedung (9).jpg">
<img src="gedung (6).jpg">
</div>

<h2>Wedding Hall</h2>
<div class="facility-images">
<img src="wedding hall.webp">
<img src="gedung (8).jpg">
<img src="gedung (9).jpg">
<img src="gedung (6).jpg">
</div>
</div>
</section>

<!-- FOOTER -->
<section id="contact">
<footer class="footer">
<div class="footer-inner">
<div>
<h2 class="brand-font">Simalem Convention Hall</h2>
<p>Venue terbaik untuk acara prestisius kamu.</p>
</div>

<div>
<h3>Alamat</h3>
<p>
Jalan Raya Jakarta–Bogor Km 48 No.46<br>
RT 01 RW 04, Cibinong<br>
Bogor, Jawa Barat
</p>
</div>

<div>
<h3>Kontak</h3>
<p>WA: <a href="https://wa.me/6282310375137">0823-1037-5137</a></p>
<p>Email: <a href="mailto:gedungsimalem@gmail.com">gedungsimalem@gmail.com</a></p>
<p>IG: <a href="https://instagram.com/simalemconventionhall">@simalemconventionhall</a></p>
</div>
</div>

<div class="footer-bottom">
© 2026 Simalem Convention Hall. All Rights Reserved.
</div>
</footer>
</section>

<!-- JS -->
<script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>
<script src="script.js"></script>

</body>
</html>

/* ================= GLOBAL ================= */
*{margin:0;padding:0;box-sizing:border-box;font-family:'Montserrat',sans-serif}
html{scroll-behavior:smooth}
body{background:#fff;color:#333;overflow-x:hidden}
section{scroll-margin-top:90px}

/* ================= HEADER ================= */
header{
    position:fixed;top:0;left:0;width:100%;z-index:999;
    display:flex;justify-content:space-between;align-items:center;
    padding:22px 40px;height:78px;background:#fff;
    transition:.4s ease
}
header.scrolled{
    padding:12px 30px;height:72px;
    box-shadow:0 4px 12px rgba(0,0,0,.08)
}
.logo img{height:110px;border-radius:12px;transition:.4s}
header.scrolled .logo img{height:80px}

nav{display:flex;gap:42px;align-items:center}
nav a{text-decoration:none;color:#000;font-weight:700;letter-spacing:1px}
nav a:hover{color:#004AAD}

.search-box{
    padding:6px 14px;border-radius:20px;
    border:1px solid #ccc;display:none
}

.header-controls{display:flex;gap:20px;align-items:center}
.icon-small{font-size:20px;cursor:pointer}
.mobile-menu-icon{display:none;font-size:26px;cursor:pointer}

/* ================= MOBILE MENU ================= */
@media(max-width:1024px){
    nav{
        display:none;flex-direction:column;
        position:absolute;top:100%;left:0;width:100%;
        background:#000
    }
    nav.active{display:flex}
    nav a{color:#fff;padding:14px;text-align:center}
    .mobile-menu-icon{display:block}
}

/* ================= SWIPER ================= */
.swiper-container{width:100%;height:100vh}
.swiper-slide video{
    width:100%;
    height:100%;
    object-fit:cover;
}

/* ===== FIX VIDEO RATIO MOBILE ===== */
@media(max-width:768px){
    .swiper-container{height:auto;aspect-ratio:9/16}
    .swiper-slide video{object-fit:contain;background:#000}
}

/* ================= SECTION ================= */
.container{
    max-width:1200px;
    margin:30px auto;
    padding:0 20px;
    text-align:center
}
.container h1{
    font-size:34px;
    color:#892900;
    margin-bottom:10px;
}

/* ================= ABOUT ================= */
.about-section p{
    max-width:900px;
    margin:15px auto;
    line-height:1.8;
    font-size:16px
}
.brand-font{
    font-family:'poppins',serif;
    font-weight:700;
    letter-spacing:1px;
}

/* ================= FACILITIES ================= */
.facility-group{margin-bottom:60px}
.facility-group h2{margin-bottom:18px;color:#c39500;font-size:22px}
.facility-images{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:20px;
}
.facility-images img{
    width:100%;
    aspect-ratio:4/5;
    object-fit:cover;
    border-radius:14px;
    box-shadow:0 6px 16px rgba(0,0,0,.12);
    background:#eee;
}
@media(max-width:1024px){.facility-images{grid-template-columns:repeat(3,1fr)}}
@media(max-width:768px){.facility-images{grid-template-columns:repeat(2,1fr)}}
@media(max-width:480px){.facility-images{grid-template-columns:1fr}}

/* ================= FOOTER ================= */
.footer{background:#ad5400;color:#fff;padding:60px 20px 20px}
.footer-inner{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:80px;
    max-width:1200px;
    margin:auto;
    text-align:left;
}
.footer h3{margin-bottom:14px;font-size:18px}
.footer p{font-size:14px;line-height:1.8;opacity:.95}
.footer a{color:#ffd89b;text-decoration:none}
.footer a:hover{text-decoration:underline}
.footer-bottom{
    border-top:1px solid rgba(255,255,255,.3);
    margin-top:40px;
    padding-top:14px;
    text-align:center;
    font-size:13px;
    opacity:.85;
}
@media(max-width:768px){
    .footer-inner{grid-template-columns:1fr;gap:30px;text-align:center}
}

new Swiper('.swiper-container',{
    direction:'vertical'
});

const header=document.getElementById('header');
const nav=document.getElementById('nav');
const mobileMenu=document.getElementById('mobileMenu');

window.addEventListener('scroll',()=>{
    header.classList.toggle('scrolled',window.scrollY>50)
});

mobileMenu.onclick=()=>nav.classList.toggle('active');

