<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SoundForge 2026 | Make a Legacy</title>
    <!-- Import Font Google untuk kesan Poster Konser & Esports Modern -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@400;700&family=Bebas+Neue&family=Inter:wght@400;600&display=swap" rel="stylesheet">
    
    <style>
        /* --- RESET & GLOBAL STYLES (60% Warna Dasar Hitam Pekat) --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #0d0d0d;
            color: #ffffff; /* Font Putih */
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
        }

        /* --- AKSEN WARNA KUNING (10%) --- */
        .text-yellow {
            color: #ffcc00 !important;
        }

        a {
            color: #ffcc00;
            text-decoration: none;
            transition: 0.3s;
        }

        a:hover {
            color: #ffea00;
        }

        .container {
            width: 85%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem 0;
        }

        /* --- NAVIGATION --- */
        header {
            background-color: #000000;
            border-bottom: 3px solid #ffcc00;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }

        /* Gaya Font Logo: Bebas Neue (Bersih & Elegan / Poster Konser) */
        .logo-wrapper {
            display: flex;
            flex-direction: column;
            line-height: 1;
        }

        .logo {
            font-family: 'Bebas Neue', sans-serif;
            font-size: 2.5rem;
            letter-spacing: 3px;
            color: #ffffff;
        }

        .logo span {
            color: #ffcc00;
        }

        .tagline-sub {
            font-family: 'Barlow Condensed', sans-serif;
            font-size: 0.9rem;
            letter-spacing: 4px;
            color: #aaaaaa;
            text-transform: uppercase;
            margin-top: 2px;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            font-family: 'Barlow Condensed', sans-serif;
            font-size: 1.2rem;
            letter-spacing: 1px;
            color: #cccccc;
            font-weight: 700;
            text-transform: uppercase;
        }

        nav ul li a:hover {
            color: #ffcc00;
        }

        /* --- HERO SECTION --- */
        .hero {
            background: linear-gradient(rgba(13, 13, 13, 0.75), rgba(13, 13, 13, 0.98)), 
                        url('https://images.unsplash.com/photo-1501386761578-eac5c94b800a?q=80&w=1200') no-repeat center center/cover;
            padding: 10rem 0;
            text-align: center;
        }

        .hero h1 {
            font-family: 'Bebas Neue', sans-serif;
            font-size: 5rem;
            letter-spacing: 4px;
            margin-bottom: 1rem;
            text-transform: uppercase;
            line-height: 0.95;
        }

        .hero p {
            font-family: 'Barlow Condensed', sans-serif;
            font-size: 1.5rem;
            letter-spacing: 1px;
            color: #dddddd;
            margin-bottom: 2.5rem;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }

        .btn {
            display: inline-block;
            background-color: #ffcc00;
            color: #000000; /* Tulisan hitam di tombol agar kontras */
            padding: 0.8rem 2.5rem;
            font-family: 'Bebas Neue', sans-serif;
            font-size: 1.4rem;
            letter-spacing: 2px;
            font-weight: bold;
            border-radius: 0px; /* Box tajam ala industrial/esports */
            text-transform: uppercase;
            border: 2px solid #ffcc00;
            cursor: pointer;
            transition: 0.3s;
        }

        .btn:hover {
            background-color: transparent;
            color: #ffcc00;
            transform: scale(1.05);
        }

        /* --- SECTION FORMATTING --- */
        .section {
            padding: 6rem 0;
            border-bottom: 1px solid #222222;
        }

        .section-title {
            font-family: 'Bebas Neue', sans-serif;
            font-size: 3rem;
            letter-spacing: 2px;
            text-align: center;
            margin-bottom: 3rem;
            text-transform: uppercase;
        }

        .section-title span {
            color: #ffcc00;
        }

        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }

        /* --- REGISTRATION SECTION --- */
        .reg-steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .step-card {
            background-color: #000000;
            padding: 3rem 2rem;
            border: 1px solid #222222;
            border-top: 4px solid #ffcc00;
            text-align: center;
        }

        .step-number {
            font-family: 'Bebas Neue', sans-serif;
            font-size: 3rem;
            color: #ffcc00;
            margin-bottom: 0.5rem;
        }

        .step-card h3 {
            font-family: 'Barlow Condensed', sans-serif;
            font-size: 1.5rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 1rem;
        }

        .step-card p {
            color: #cccccc;
            font-size: 0.95rem;
        }

        .reg-action {
            text-align: center;
            margin-top: 4rem;
        }

        /* --- ARCHIVE TABLE --- */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 2rem;
            background-color: #000000;
            border: 1px solid #222222;
        }

        th, td {
            padding: 1.2rem 1.5rem;
            text-align: left;
        }

        th {
            background-color: #111111;
            color: #ffcc00;
            font-family: 'Barlow Condensed', sans-serif;
            font-size: 1.2rem;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 1px;
            border-bottom: 2px solid #ffcc00;
        }

        td {
            font-size: 1rem;
            border-bottom: 1px solid #222222;
        }

        tr:hover {
            background-color: #111111;
        }

        /* --- FOOTER --- */
        footer {
            background-color: #000000;
            text-align: center;
            padding: 3rem 0;
            color: #666666;
            font-size: 0.9rem;
            border-top: 2px solid #222222;
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
                gap: 1.5rem;
            }
            nav ul li {
                margin: 0 1rem;
            }
            .grid-2 {
                grid-template-columns: 1fr;
                gap: 2.5rem;
            }
            .hero h1 {
                font-size: 3.5rem;
            }
        }
    </style>
</head>
<body>

    <!-- NAVIGASI UTAMA -->
    <header>
        <div class="container nav-container">
            <div class="logo-wrapper">
                <div class="logo">SOUND<span>FORGE</span></div>
                <div class="tagline-sub">Make a Legacy</div>
            </div>
            <nav>
                <ul>
                    <li><a href="#konsep">Konsep</a></li>
                    <li><a href="#pendaftaran">Pendaftaran</a></li>
                    <li><a href="#arsip">Arsip Event</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- HERO BANNER -->
    <section class="hero">
        <div class="container">
            <h1>all genre, all style, one stage</h1>
            <p>Bawa karya terbaikmu, dan ciptakan penampilan yang layak dikenang.</p>
            <a href="#pendaftaran" class="btn">Daftar Sekarang</a>
        </div>
    </section>

    <!-- KONSEP EVENT -->
    <section id="konsep" class="section">
        <div class="container">
            <h2 class="section-title">Konsep <span>SoundForge</span></h2>
            <div class="grid-2">
                <div>
                    <p style="font-size: 1.2rem; margin-bottom: 1.5rem; font-weight: 600;">
                        SoundForge bukan sekadar festival musik biasa. Ini adalah ruang penempaan bagi band yang siap mengukir sejarah baru di industri musik.
                    </p>
                    <p style="color: #cccccc;">
                        Kami percaya kebebasan berekspresi adalah kunci. Di panggung ini, penilaian tidak dibatasi oleh sekat-sekat genre, melainkan orisinalitas, karakter penampilan, kedalaman lirik, serta energi yang dilepaskan di atas panggung.
                    </p>
                </div>
                <div style="background-color: #000000; padding: 2.5rem; border: 1px solid #222222; border-left: 4px solid #ffcc00;">
                    <h3 style="margin-bottom: 1.5rem; font-family: 'Barlow Condensed', sans-serif; font-size: 1.6rem; text-transform: uppercase; letter-spacing: 1px;">Benefit Kompetisi:</h3>
                    <ul style="list-style-position: inside; color: #cccccc; line-height: 2;">
                        <li><span class="text-yellow">✔</span> Kontrak Rekaman Single Digital</li>
                        <li><span class="text-yellow">✔</span> Hadiah Tunai Total Puluhan Juta Rupiah</li>
                        <li><span class="text-yellow">✔</span> Eksklusif Mentoring Bersama Musisi Nasional</li>
                        <li><span class="text-yellow">✔</span> Main Slot di Festival Utama SoundForge</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- PENDAFTARAN -->
    <section id="pendaftaran" class="section">
        <div class="container">
            <h2 class="section-title">Alur <span>Pendaftaran</span></h2>
            <div class="reg-steps">
                <div class="step-card">
                    <div class="step-number">01</div>
                    <h3>Unduh Regulasi</h3>
                    <p>Pelajari panduan lengkap kompetisi, persyaratan aransemen lagu, serta ketentuan teknis lainnya.</p>
                </div>
                <div class="step-card">
                    <div class="step-number">02</div>
                    <h3>Kirim Demo</h3>
                    <p>Unggah 1 video rekaman penampilan live terbaik band Anda ke platform YouTube (Unlisted/Public).</p>
                </div>
                <div class="step-card">
                    <div class="step-number">03</div>
                    <h3>Isi Formulir</h3>
                    <p>Lengkapi data seluruh personil band serta cantumkan tautan video demo Anda pada formulir resmi.</p>
                </div>
            </div>
            <div class="reg-action">
                <a href="#" class="btn" target="_blank">Buka Formulir Pendaftaran</a>
            </div>
        </div>
    </section>

    <!-- ARSIP EVENT -->
    <section id="arsip" class="section">
        <div class="container">
            <h2 class="section-title">Catatan <span>Arsip Event</span></h2>
            <p style="text-align: center; color: #cccccc; max-width: 600px; margin: -2rem auto 3rem auto; font-family: 'Barlow Condensed', sans-serif; font-size: 1.3rem; letter-spacing: 0.5px;">Rekam jejak para juara dari edisi terdahulu yang kini telah merajai panggung industri musik.</p>
            
            <div style="overflow-x: auto;">
                <table>
                    <thead>
                        <tr>
                            <th>Tahun</th>
                            <th>Jawara 1</th>
                            <th>Genre</th>
                            <th>Kota Asal</th>
                            <th>Status Sekarang</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>2025</td>
                            <td style="font-weight: bold; color: #ffcc00;">Distorsi Senja</td>
                            <td>Alternative Rock</td>
                            <td>Bandung</td>
                            <td>Tur Album Pertama</td>
                        </tr>
                        <tr>
                            <td>2024</td>
                            <td style="font-weight: bold; color: #ffcc00;">Iron Pulse</td>
                            <td>Heavy Metal</td>
                            <td>Jakarta</td>
                            <td>Aktif di Platform Digital</td>
                        </tr>
                        <tr>
                            <td>2023</td>
                            <td style="font-weight: bold; color: #ffcc00;">The Midnight Echo</td>
                            <td>Indie Pop</td>
                            <td>Yogyakarta</td>
                            <td>Kontrak Label Nasional</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <div class="container">
            <p style="font-family: 'Barlow Condensed', sans-serif; font-size: 1.1rem; letter-spacing: 1px; color: #ffffff;">&copy; 2026 SOUNDFORGE MUSIC OFFICIAL. ALL RIGHTS RESERVED.</p>
            <p style="margin-top: 0.5rem; font-size: 0.8rem; color: #555555; letter-spacing: 2px; text-transform: uppercase;">Make a Legacy</p>
        </div>
    </footer>

</body>
</html>
