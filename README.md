<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SoundForge 2026 | Official Band Competition</title>
    <style>
        /* --- RESET & GLOBAL STYLES --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #0b0b0d;
            color: #e2e8f0;
            line-height: 1.6;
        }

        a {
            color: #ff0055;
            text-decoration: none;
            transition: 0.3s;
        }

        a:hover {
            color: #ff5599;
        }

        .container {
            width: 85%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem 0;
        }

        /* --- NAVIGATION --- */
        header {
            background-color: #121216;
            border-bottom: 2px solid #ff0055;
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

        .logo {
            font-size: 1.8rem;
            font-weight: 800;
            letter-spacing: 2px;
            color: #fff;
        }

        .logo span {
            color: #ff0055;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            color: #a0aec0;
            font-weight: 600;
        }

        nav ul li a:hover {
            color: #fff;
        }

        /* --- HERO SECTION --- */
        .hero {
            background: linear-gradient(rgba(11, 11, 13, 0.8), rgba(11, 11, 13, 0.95)), 
                        url('https://images.unsplash.com/photo-1501386761578-eac5c94b800a?q=80&w=1200') no-repeat center center/cover;
            padding: 8rem 0;
            text-align: center;
        }

        .hero h1 {
            font-size: 3.5rem;
            font-weight: 900;
            letter-spacing: 3px;
            margin-bottom: 1rem;
            text-transform: uppercase;
        }

        .hero p {
            font-size: 1.2rem;
            color: #a0aec0;
            margin-bottom: 2rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .btn {
            display: inline-block;
            background-color: #ff0055;
            color: #fff;
            padding: 0.8rem 2rem;
            font-weight: bold;
            border-radius: 5px;
            text-transform: uppercase;
            letter-spacing: 1px;
            border: none;
            cursor: pointer;
        }

        .btn:hover {
            background-color: #e6004c;
            transform: translateY(-2px);
            color: #fff;
        }

        /* --- CONCEPT SECTION --- */
        .section {
            padding: 5rem 0;
            border-bottom: 1px solid #1a1a24;
        }

        .section-title {
            font-size: 2.2rem;
            text-align: center;
            margin-bottom: 3rem;
            text-transform: uppercase;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 50px;
            height: 4px;
            background-color: #ff0055;
            margin: 10px auto 0 auto;
        }

        .grid-2 {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            align-items: center;
        }

        /* --- REGISTRATION SECTION --- */
        .reg-steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .step-card {
            background-color: #121216;
            padding: 2.5rem 2rem;
            border-radius: 8px;
            border-top: 4px solid #ff0055;
            text-align: center;
        }

        .step-number {
            font-size: 2.5rem;
            font-weight: 900;
            color: #ff0055;
            margin-bottom: 1rem;
        }

        .step-card h3 {
            margin-bottom: 1rem;
        }

        .reg-action {
            text-align: center;
            margin-top: 3rem;
        }

        /* --- ARCHIVE SECTION --- */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 2rem;
            background-color: #121216;
            border-radius: 8px;
            overflow: hidden;
        }

        th, td {
            padding: 1rem 1.5rem;
            text-align: left;
        }

        th {
            background-color: #1a1a24;
            color: #ff0055;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        tr {
            border-bottom: 1px solid #1a1a24;
        }

        tr:last-child {
            border-bottom: none;
        }

        tr:hover {
            background-color: #16161f;
        }

        /* --- FOOTER --- */
        footer {
            background-color: #070709;
            text-align: center;
            padding: 2rem 0;
            color: #4a5568;
            font-size: 0.9rem;
            border-top: 1px solid #1a1a24;
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
                gap: 1rem;
            }
            nav ul li {
                margin: 0 1rem;
            }
            .grid-2 {
                grid-template-columns: 1fr;
                gap: 2rem;
            }
            .hero h1 {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>

    <!-- NAVIGASI -->
    <header>
        <div class="container nav-container">
            <div class="logo">SOUND<span>FORGE</span></div>
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
            <h1>Tempa Karakter Bandmu</h1>
            <p>Kompetisi band indie terbesar tahun ini. Saatnya menunjukkan distorsi, harmoni, dan aksi panggung terbaikmu di hadapan para produser musik nasional.</p>
            <a href="#pendaftaran" class="btn">Daftar Sekarang</a>
        </div>
    </section>

    <!-- KONSEP EVENT -->
    <section id="konsep" class="section">
        <div class="container">
            <h2 class="section-title">Konsep SoundForge</h2>
            <div class="grid-2">
                <div>
                    <p style="font-size: 1.1rem; margin-bottom: 1.5rem;">
                        <strong>SoundForge</strong> bukan sekadar festival musik biasa. Ini adalah wadah pencarian bakat bagi band-band lokal untuk "ditempa" menjadi unit musik yang solid, profesional, dan siap industri.
                    </p>
                    <p style="color: #a0aec0;">
                        Kami percaya bahwa setiap band memiliki identitas unik. Di SoundForge, penilaian tidak hanya diambil dari kelihaian bermain instrumen, namun juga originalitas lagu, aksi panggung (*stage act*), serta kedalaman lirik. Genre terbuka lebar bagi unit Rock, Metal, Pop, Jazz, hingga Elektronik.
                    </p>
                </div>
                <div style="background-color: #121216; padding: 2rem; border-radius: 8px; border-left: 4px solid #ff0055;">
                    <h3 style="margin-bottom: 1rem; color: #fff;">Yang Kamu Dapatkan:</h3>
                    <ul style="list-style-position: inside; color: #a0aec0;">
                        <li style="margin-bottom: 0.5rem;">Kontrak Rekaman Single Digital</li>
                        <li style="margin-bottom: 0.5rem;">Hadiah Tunai Total Puluhan Juta Rupiah</li>
                        <li style="margin-bottom: 0.5rem;">Sesi Mentoring Bersama Musisi Senior</li>
                        <li style="margin-bottom: 0.5rem;">Slot Tampil di Festival SoundForge Utama</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- PENDAFTARAN -->
    <section id="pendaftaran" class="section">
        <div class="container">
            <h2 class="section-title">Alur Pendaftaran</h2>
            <div class="reg-steps">
                <div class="step-card">
                    <div class="step-number">01</div>
                    <h3>Unduh Regulasi</h3>
                    <p style="color: #a0aec0; font-size: 0.95rem;">Pelajari booklet syarat, ketentuan lagu orisinal/cover, dan detail teknis kompetisi.</p>
                </div>
                <div class="step-card">
                    <div class="step-number">02</div>
                    <h3>Kirim Demo</h3>
                    <p style="color: #a0aec0; font-size: 0.95rem;">Unggah 1 video live perform band Anda ke YouTube (Unlisted/Public) sebagai materi seleksi awal.</p>
                </div>
                <div class="step-card">
                    <div class="step-number">03</div>
                    <h3>Isi Formulir</h3>
                    <p style="color: #a0aec0; font-size: 0.95rem;">Lengkapi data anggota band dan sematkan link video demo pada tombol pendaftaran di bawah.</p>
                </div>
            </div>
            <div class="reg-action">
                <!-- Ganti tanda pagar (#) di bawah dengan link Google Form pendaftaran Anda jika ada -->
                <a href="#" class="btn" target="_blank">Buka Formulir Pendaftaran</a>
            </div>
        </div>
    </section>

    <!-- ARSIP EVENT -->
    <section id="arsip" class="section">
        <div class="container">
            <h2 class="section-title">Catatan Arsip Event</h2>
            <p style="text-align: center; color: #a0aec0; max-width: 600px; margin: -2rem auto 2rem auto;">Perjalanan SoundForge dari tahun ke tahun melahirkan jawara baru yang kini meramaikan industri musik tanah air.</p>
            
            <div style="overflow-x: auto;">
                <table>
                    <thead>
                        <tr>
                            <th>Tahun</th>
                            <th>Juara 1</th>
                            <th>Genre</th>
                            <th>Kota Asal</th>
                            <th>Status Sekarang</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>2025</td>
                            <td><strong>Distorsi Senja</strong></td>
                            <td>Alternative Rock</td>
                            <td>Bandung</td>
                            <td>Tur Album Pertama</td>
                        </tr>
                        <tr>
                            <td>2024</td>
                            <td><strong>Iron Pulse</strong></td>
                            <td>Heavy Metal</td>
                            <td>Jakarta</td>
                            <td>Aktif di Spotify</td>
                        </tr>
                        <tr>
                            <td>2023</td>
                            <td><strong>The Midnight Echo</strong></td>
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
            <p>&copy; 2026 SoundForge Music Official. All Rights Reserved.</p>
            <p style="margin-top: 0.5rem; font-size: 0.8rem;">Dibuat dengan semangat independen.</p>
        </div>
    </footer>

</body>
</html>
