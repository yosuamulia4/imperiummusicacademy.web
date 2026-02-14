<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IMPERIUM Music Academy | Elevate Your Rhythm</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    
    <style>
        /* --- CSS INTERNAL --- */
        :root {
            --primary-color: #38bdf8; /* Biru Cerah Profesional */
            --bg-dark: #0f172a;
            --bg-card: #1e293b;
            --text-light: #f8fafc;
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-light);
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 8%;
            background: rgba(15, 23, 42, 0.95);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid rgba(255,255,255,0.1);
        }

        .logo {
            font-size: 24px;
            font-weight: 700;
            letter-spacing: 1px;
            text-transform: uppercase;
        }

        .logo span { color: var(--primary-color); }

        nav ul {
            display: flex;
            list-style: none;
            align-items: center;
        }

        nav ul li { margin-left: 30px; }

        nav ul li a {
            text-decoration: none;
            color: #fff;
            font-size: 14px;
            font-weight: 500;
            transition: var(--transition);
        }

        nav ul li a:hover { color: var(--primary-color); }

        .btn-nav {
            background: var(--primary-color);
            padding: 10px 22px;
            border-radius: 50px;
            color: #fff !important;
            font-weight: 600;
        }

        /* Hero Section */
        header {
            height: 100vh;
            background: linear-gradient(rgba(15, 23, 42, 0.8), rgba(15, 23, 42, 0.8)), 
                        url('https://images.unsplash.com/photo-1511671782779-c97d3d27a1d4?auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding-top: 80px;
        }

        .hero-content h1 {
            font-size: clamp(2.5rem, 5vw, 4rem);
            margin-bottom: 20px;
            line-height: 1.2;
        }

        .hero-content p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
            color: #94a3b8;
        }

        .main-btn {
            display: inline-block;
            padding: 15px 40px;
            background: var(--primary-color);
            color: #fff;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 700;
            transition: var(--transition);
            box-shadow: 0 10px 20px rgba(56, 189, 248, 0.2);
        }

        .main-btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(56, 189, 248, 0.4);
        }

        /* Section Styling */
        section { padding: 100px 8%; }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 50px;
        }

        .section-title span { color: var(--primary-color); }

        /* Classes/Services Grid */
        .container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .card {
            background: var(--bg-card);
            padding: 40px;
            border-radius: 20px;
            text-align: center;
            transition: var(--transition);
            border: 1px solid rgba(255,255,255,0.05);
        }

        .card:hover {
            transform: translateY(-10px);
            border-color: var(--primary-color);
            background: #243147;
        }

        .card i {
            font-size: 3.5rem;
            color: var(--primary-color);
            margin-bottom: 25px;
        }

        .card h3 { margin-bottom: 15px; font-size: 1.5rem; }

        /* Pricing/Classes Info */
        .info-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
            margin-top: 40px;
        }

        .info-tag {
            background: rgba(56, 189, 248, 0.1);
            color: var(--primary-color);
            padding: 8px 20px;
            border-radius: 50px;
            font-size: 0.9rem;
            font-weight: 600;
        }

        /* Footer */
        footer {
            background: #020617;
            padding: 60px 8% 30px;
            text-align: center;
            border-top: 1px solid rgba(255,255,255,0.05);
        }

        .socials { margin: 30px 0; }
        .socials a {
            color: #fff;
            font-size: 1.8rem;
            margin: 0 15px;
            transition: var(--transition);
        }

        .socials a:hover { color: var(--primary-color); }

        .copyright {
            font-size: 0.9rem;
            color: #64748b;
        }

        /* Responsive Mobile */
        @media (max-width: 768px) {
            nav ul { display: none; } /* Simpel untuk versi 1.0 */
            .hero-content h1 { font-size: 2.5rem; }
            section { padding: 60px 5%; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">IMPERIUM <span>MUSIC</span></div>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#program">Program</a></li>
            <li><a href="#about">Tentang</a></li>
            <li><a href="https://wa.me/6285185443185" class="btn-nav">Daftar Sekarang</a></li>
        </ul>
    </nav>

    <header id="home">
        <div class="hero-content">
            <h1>Elevate Your Musical Talent</h1>
            <p>Bimbel Musik Profesional di Batam. Kuasai instrumen favoritmu dengan kurikulum yang praktis dan menyenangkan.</p>
            <a href="#program" class="main-btn">Cek Program Kami <i class="fas fa-arrow-right"></i></a>
        </div>
    </header>

    <section id="program">
        <h2 class="section-title">Program <span>Pilihan</span></h2>
        <div class="container">
            <div class="card">
                <i class="fas fa-guitar"></i>
                <h3>Gitar & Bass</h3>
                <p>Mulai dari pengenalan chord hingga teknik melodi dan improvisasi untuk pelayanan atau perform.</p>
                <div class="info-grid">
                    <span class="info-tag">Offline</span>
                    <span class="info-tag">Online</span>
                </div>
            </div>

            <div class="card">
                <i class="fas fa-drum"></i>
                <h3>Drum Academy</h3>
                <p>Pelajari teknik dasar rudiment, groove, hingga fill-in drum yang solid untuk berbagai genre.</p>
                <div class="info-grid">
                    <span class="info-tag">Offline Only</span>
                </div>
            </div>

            <div class="card">
                <i class="fas fa-video"></i>
                <h3>Interactive Online</h3>
                <p>Belajar langsung dari rumah via Zoom/Gmeet dengan jadwal yang fleksibel bagi pekerja atau pelajar.</p>
                <div class="info-grid">
                    <span class="info-tag">E-Certificate</span>
                </div>
            </div>
        </div>
    </section>

    <section id="about" style="background: #0a101f;">
        <div style="max-width: 800px; margin: 0 auto; text-align: center;">
            <h2 class="section-title">Mengapa <span>IMPERIUM?</span></h2>
            <p style="color: #94a3b8; font-size: 1.1rem; margin-bottom: 20px;">
                Kami percaya setiap orang punya potensi musik. Dengan pengajar yang aktif di bidang pelayanan gereja dan industri musik, kami memastikan Anda tidak hanya sekedar "bisa main", tapi paham esensi musik itu sendiri.
            </p>
            <div style="display: flex; justify-content: center; gap: 40px; margin-top: 40px;">
                <div>
                    <h4 style="color: var(--primary-color); font-size: 2rem;">100%</h4>
                    <p>Praktis</p>
                </div>
                <div>
                    <h4 style="color: var(--primary-color); font-size: 2rem;">Flexible</h4>
                    <p>Jadwal</p>
                </div>
                <div>
                    <h4 style="color: var(--primary-color); font-size: 2rem;">Privat</h4>
                    <p>Fokus</p>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="logo">IMPERIUM <span>MUSIC ACADEMY</span></div>
        <p style="margin-top: 10px; color: #94a3b8;"> Batam - Kepulauan Riau</p>
        
        <div class="socials">
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-whatsapp"></i></a>
            <a href="#"><i class="fab fa-youtube"></i></a>
        </div>
        
        <div class="copyright">
            &copy; 2026 IMPERIUM Group. Founder: <strong>Yosua Sinaga</strong>.
        </div>
    </footer>

</body>
</html>
