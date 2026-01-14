# Ceylon-Island-Vibe
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Ceylon Island Vibe - Experience the soul of Sri Lanka. Luxury stays, authentic cultural tours, and unforgettable adventures.">
    <meta name="keywords" content="Sri Lanka Travel, Ceylon Tours, Luxury Holidays, Sri Lanka Hotels, Tea Trails, Safari Sri Lanka">
    <meta name="author" content="Ceylon Island Vibe">
    <title>Ceylon Island Vibe | Luxury Travel &amp; Experiences</title>

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&amp;family=Playfair+Display:wght@400;700&amp;display=swap" rel="stylesheet">
    
    <!-- Font Awesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        /* =========================================
           CSS VARIABLES & RESET
           ========================================= */
        :root {
            --primary-color: #064e3b; /* Emerald Green */
            --primary-light: #10b981;
            --accent-color: #d97706; /* Gold/Amber */
            --text-dark: #1f2937;
            --text-light: #6b7280;
            --bg-light: #f9fafb;
            --white: #ffffff;
            --transition: all 0.3s ease;
            --shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Inter', sans-serif;
            color: var(--text-dark);
            line-height: 1.6;
            overflow-x: hidden;
            background-color: var(--white);
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Playfair Display', serif;
            color: var(--primary-color);
            margin-bottom: 1rem;
        }

        a {
            text-decoration: none;
            color: inherit;
            transition: var(--transition);
        }

        ul {
            list-style: none;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        /* Utility Classes */
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        .section-padding {
            padding: 80px 0;
        }

        .text-center { text-align: center; }
        
        .section-title {
            font-size: 2.5rem;
            margin-bottom: 10px;
            position: relative;
            display: inline-block;
        }

        .section-subtitle {
            color: var(--accent-color);
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-size: 0.9rem;
            display: block;
            margin-bottom: 10px;
        }

        .btn {
            display: inline-block;
            padding: 12px 30px;
            border-radius: 50px;
            font-weight: 600;
            cursor: pointer;
            border: 2px solid transparent;
            transition: var(--transition);
        }

        .btn-primary {
            background-color: var(--primary-color);
            color: var(--white);
        }

        .btn-primary:hover {
            background-color: var(--primary-light);
            transform: translateY(-2px);
        }

        .btn-outline {
            border-color: var(--white);
            color: var(--white);
            background: rgba(255,255,255,0.1);
            backdrop-filter: blur(5px);
        }

        .btn-outline:hover {
            background-color: var(--white);
            color: var(--primary-color);
        }

        .btn-book {
            background-color: var(--accent-color);
            color: var(--white);
            font-size: 0.9rem;
            text-align: center;
            padding: 10px 25px;
        }
        
        .btn-book:hover {
            background-color: #b45309;
        }

        /* =========================================
           HEADER & NAVIGATION
           ========================================= */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            padding: 20px 0;
            transition: var(--transition);
        }

        header.scrolled {
            background-color: var(--white);
            box-shadow: var(--shadow);
            padding: 15px 0;
        }

        header.scrolled .logo {
            color: var(--primary-color);
        }

        header.scrolled .nav-link {
            color: var(--text-dark);
        }

        header.scrolled .hamburger div {
            background-color: var(--text-dark);
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--white);
            letter-spacing: 1px;
        }

        .nav-menu {
            display: flex;
            align-items: center;
            gap: 30px;
        }

        .nav-link {
            color: var(--white);
            font-weight: 500;
            font-size: 0.95rem;
            position: relative;
        }

        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -5px;
            left: 0;
            background-color: var(--accent-color);
            transition: var(--transition);
        }

        .nav-link:hover::after {
            width: 100%;
        }

        /* Language Toggle */
        .lang-toggle {
            display: flex;
            gap: 5px;
            margin-left: 20px;
        }

        .lang-btn {
            background: none;
            border: none;
            color: var(--white);
            font-size: 0.8rem;
            font-weight: bold;
            cursor: pointer;
            opacity: 0.7;
        }

        header.scrolled .lang-btn { color: var(--text-dark); }
        .lang-btn.active { opacity: 1; text-decoration: underline; }

        /* Hamburger */
        .hamburger {
            display: none;
            cursor: pointer;
        }

        .hamburger div {
            width: 25px;
            height: 3px;
            background-color: var(--white);
            margin: 5px;
            transition: var(--transition);
        }

        /* =========================================
           HERO SECTION
           ========================================= */
        #hero {
            height: 100vh;
            /* REPLACE WITH YOUR OWN HERO IMAGE BELOW */
            background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.5)), 
                        url('https://picsum.photos/seed/srilankabeachvibe/1920/1080.jpg') center/cover no-repeat;
            background-attachment: fixed; 
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--white);
            position: relative;
            overflow: hidden;
        }

        /* Animation for Hero Background */
        @keyframes zoomEffect {
            0% { transform: scale(1); }
            100% { transform: scale(1.1); }
        }

        #hero::before {
            content: '';
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            background: inherit;
            z-index: -1;
            animation: zoomEffect 20s infinite alternate;
        }

        .hero-content {
            max-width: 800px;
            padding: 20px;
            z-index: 1;
        }

        .hero-title {
            font-size: 3.5rem;
            margin-bottom: 20px;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeUp 1s forwards 0.5s;
        }

        .hero-text {
            font-size: 1.2rem;
            margin-bottom: 30px;
            opacity: 0;
            transform: translateY(30px);
            animation: fadeUp 1s forwards 0.8s;
        }

        .hero-btns {
            opacity: 0;
            animation: fadeUp 1s forwards 1.1s;
            display: flex;
            gap: 15px;
            justify-content: center;
        }

        @keyframes fadeUp {
            to { opacity: 1; transform: translateY(0); }
        }

        /* =========================================
           SECTIONS (Stays, Experiences, etc.)
           ========================================= */
        
        /* Grid Layouts */
        .grid-3 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        /* Cards */
        .card {
            background: var(--white);
            border-radius: 12px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            position: relative;
            display: flex;
            flex-direction: column;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }

        .card-img-wrapper {
            overflow: hidden;
            height: 250px;
        }

        .card-img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .card:hover .card-img {
            transform: scale(1.1);
        }

        .card-content {
            padding: 25px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .card-meta {
            font-size: 0.85rem;
            color: var(--accent-color);
            margin-bottom: 10px;
            display: block;
        }

        /* About Section */
        #about {
            background-color: var(--bg-light);
        }
        
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        /* Gallery Section */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
        }

        .gallery-item {
            cursor: pointer;
            overflow: hidden;
            border-radius: 8px;
            height: 250px;
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }

        .gallery-item:hover img {
            transform: scale(1.05);
            filter: brightness(0.8);
        }

        /* Testimonials */
        #testimonials {
            background-color: var(--primary-color);
            color: var(--white);
        }

        #testimonials .section-title, #testimonials h2 {
            color: var(--white);
        }

        .testimonial-card {
            background: rgba(255,255,255,0.1);
            backdrop-filter: blur(10px);
            padding: 30px;
            border-radius: 10px;
            border: 1px solid rgba(255,255,255,0.2);
        }

        .stars { color: var(--accent-color); margin-bottom: 15px; }

        /* Contact Form */
        .contact-wrapper {
            background: var(--white);
            padding: 40px;
            border-radius: 12px;
            box-shadow: var(--shadow);
            max-width: 600px;
            margin: 0 auto;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }

        .form-control {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 6px;
            font-family: inherit;
            transition: var(--transition);
        }

        .form-control:focus {
            outline: none;
            border-color: var(--primary-color);
            box-shadow: 0 0 0 3px rgba(6, 78, 59, 0.1);
        }

        /* Footer */
        footer {
            background-color: #111827;
            color: #d1d5db;
            padding: 60px 0 20px;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-logo {
            color: var(--white);
            font-family: 'Playfair Display', serif;
            font-size: 1.5rem;
            margin-bottom: 15px;
            display: inline-block;
        }

        .footer-links li { margin-bottom: 10px; }
        .footer-links a:hover { color: var(--primary-light); }

        .social-icons { display: flex; gap: 15px; }
        .social-icons a {
            width: 40px; height: 40px;
            background: rgba(255,255,255,0.1);
            display: flex; align-items: center; justify-content: center;
            border-radius: 50%;
            transition: var(--transition);
        }
        .social-icons a:hover { background: var(--primary-color); color: var(--white); }

        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            font-size: 0.9rem;
        }

        /* =========================================
           EXTRAS (Lightbox, Toast, WhatsApp)
           ========================================= */
        
        /* Lightbox */
        .lightbox {
            position: fixed;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: rgba(0,0,0,0.9);
            z-index: 2000;
            display: none;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .lightbox.active { display: flex; animation: fadeIn 0.3s; }

        .lightbox-img {
            max-width: 90%;
            max-height: 90vh;
            border-radius: 5px;
            box-shadow: 0 0 20px rgba(0,0,0,0.5);
        }

        .lightbox-close {
            position: absolute;
            top: 20px;
            right: 30px;
            color: var(--white);
            font-size: 2rem;
            cursor: pointer;
        }

        /* Toast Notification */
        #toast {
            visibility: hidden;
            min-width: 250px;
            background-color: #333;
            color: #fff;
            text-align: center;
            border-radius: 4px;
            padding: 16px;
            position: fixed;
            z-index: 3000;
            left: 50%;
            bottom: 30px;
            transform: translateX(-50%);
            font-size: 17px;
        }

        #toast.show {
            visibility: visible;
            animation: fadein 0.5s, fadeout 0.5s 2.5s;
        }

        /* WhatsApp Float */
        .whatsapp-float {
            position: fixed;
            width: 60px;
            height: 60px;
            bottom: 40px;
            right: 40px;
            background-color: #25d366;
            color: #FFF;
            border-radius: 50px;
            text-align: center;
            font-size: 30px;
            box-shadow: 2px 2px 3px #999;
            z-index: 1000;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
        }

        .whatsapp-float:hover {
            background-color: #128c7e;
            transform: scale(1.1);
        }

        /* Animations */
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
        @keyframes fadein { from {bottom: 0; opacity: 0;} to {bottom: 30px; opacity: 1;} }
        @keyframes fadeout { from {bottom: 30px; opacity: 1;} to {bottom: 0; opacity: 0;} }

        /* Reveal on Scroll Class */
        .reveal {
            position: relative;
            transform: translateY(50px);
            opacity: 0;
            transition: 1s all ease;
        }
        .reveal.active {
            transform: translateY(0);
            opacity: 1;
        }

        /* =========================================
           RESPONSIVE
           ========================================= */
        @media screen and (max-width: 768px) {
            .hamburger { display: block; z-index: 1001; }
            
            .nav-menu {
                position: fixed;
                top: 0;
                right: -100%;
                width: 70%;
                height: 100vh;
                background-color: var(--white);
                flex-direction: column;
                justify-content: center;
                box-shadow: -5px 0 15px rgba(0,0,0,0.1);
                transition: 0.4s ease;
            }

            .nav-menu.active { right: 0; }
            
            .nav-link { color: var(--text-dark); font-size: 1.2rem; }
            .lang-toggle { color: var(--text-dark); margin: 20px 0; }
            
            .hero-title { font-size: 2.5rem; }
            .about-grid { grid-template-columns: 1fr; }
            .hero-btns { flex-direction: column; }
            
            .whatsapp-float {
                width: 50px; height: 50px;
                font-size: 25px;
                bottom: 20px; right: 20px;
            }
        }
    </style>
</head>
<body>

    <!-- Notification Toast -->
    <div id="toast">Message Sent! We will contact you soon.</div>

    <!-- Header -->
    <header id="header">
        <div class="container nav-container">
            <a href="#" class="logo">Ceylon Island Vibe</a>
            
            <nav>
                <ul class="nav-menu" id="nav-menu">
                    <li><a href="#hero" class="nav-link" data-i18n="home">Home</a></li>
                    <li><a href="#stays" class="nav-link" data-i18n="stays">Stays</a></li>
                    <li><a href="#experiences" class="nav-link" data-i18n="experiences">Experiences</a></li>
                    <li><a href="#gallery" class="nav-link" data-i18n="gallery">Gallery</a></li>
                    <li><a href="#contact" class="nav-link" data-i18n="contact">Contact</a></li>
                    
                    <!-- Language Toggle -->
                    <div class="lang-toggle">
                        <button class="lang-btn active" onclick="setLanguage('en')">EN</button>
                        <button class="lang-btn" onclick="setLanguage('de')">DE</button>
                        <button class="lang-btn" onclick="setLanguage('fr')">FR</button>
                    </div>
                </ul>
            </nav>

            <div class="hamburger" id="hamburger">
                <div class="line1"></div>
                <div class="line2"></div>
                <div class="line3"></div>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="hero">
        <div class="hero-content">
            <h1 class="hero-title" data-i18n="hero_title" style="color: #ffffff;">Discover the Soul of Sri Lanka</h1>
            <p class="hero-text" data-i18n="hero_subtitle">From golden beaches to misty tea plantations, experience the journey of a lifetime.</p>
            <div class="hero-btns">
                <!-- Link to Stays Section -->
                <a href="#stays" class="btn btn-primary" data-i18n="explore_stays">Explore Stays</a>
                <!-- Link to Contact/Booking -->
                <a href="#contact" class="btn btn-outline" data-i18n="plan_adventure">Plan Your Adventure</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section-padding">
        <div class="container reveal">
            <div class="text-center">
                <span class="section-subtitle" data-i18n="our_story">Our Story</span>
                <h2 class="section-title" data-i18n="about_title">Authentic Ceylonese Hospitality</h2>
            </div>
            <div class="about-grid" style="margin-top: 40px;">
                <div>
                    <!-- REPLACE WITH YOUR OWN IMAGE: e.g. 'images/tea-plantation.jpg' -->
                    <img src="https://picsum.photos/seed/ceylonteaplantation/600/400.jpg" alt="Tea Plantation Sri Lanka" style="border-radius: 10px; box-shadow: var(--shadow);">
                </div>
                <div>
                    <p style="margin-bottom: 20px;" data-i18n="about_p1">At Ceylon Island Vibe, we don't just offer trips; we curate memories. Rooted in the rich culture and natural beauty of Sri Lanka, our mission is to show travelers the hidden gems of the pearl of the Indian Ocean.</p>
                    <p data-i18n="about_p2">Whether you seek the tranquility of ancient temples, the thrill of a leopard safari, or the warmth of local cuisine, we ensure your experience is seamless, sustainable, and unforgettable.</p>
                    <div style="margin-top: 30px; display: flex; gap: 20px;">
                        <div>
                            <h3 style="color: var(--accent-color); font-size: 2rem;">500+</h3>
                            <span>Happy Travelers</span>
                        </div>
                        <div>
                            <h3 style="color: var(--accent-color); font-size: 2rem;">50+</h3>
                            <span>Locations</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Stays Section -->
    <section id="stays" class="section-padding">
        <div class="container reveal">
            <div class="text-center">
                <span class="section-subtitle" data-i18n="accommodation">Accommodation</span>
                <h2 class="section-title" data-i18n="stays_title">Curated Luxury Stays</h2>
            </div>
            
            <div class="grid-3">
                <!-- Stay 1 -->
                <article class="card">
                    <div class="card-img-wrapper">
                        <!-- REPLACE WITH YOUR OWN IMAGE -->
                        <img src="https://picsum.photos/seed/bentotavilla2/400/300.jpg" alt="Bentota Beach Villa" class="card-img">
                    </div>
                    <div class="card-content">
                        <span class="card-meta">South Coast</span>
                        <h3>Ocean Villa Bentota</h3>
                        <p style="font-size: 0.9rem; margin: 10px 0; color: var(--text-light);">Wake up to the sound of waves in this private beachfront villa featuring a infinity pool.</p>
                        <!-- Link to Contact to Book -->
                        <a href="#contact" class="btn btn-book">Book Now</a>
                    </div>
                </article>

                <!-- Stay 2 -->
                <article class="card">
                    <div class="card-img-wrapper">
                        <!-- REPLACE WITH YOUR OWN IMAGE -->
                        <img src="https://picsum.photos/seed/ellamountainview/400/300.jpg" alt="Ella Eco Lodge" class="card-img">
                    </div>
                    <div class="card-content">
                        <span class="card-meta">Hill Country</span>
                        <h3>Ella Mountain Lodge</h3>
                        <p style="font-size: 0.9rem; margin: 10px 0; color: var(--text-light);">A cozy eco-lodge nestled in the clouds, perfect for hiking and tea trail enthusiasts.</p>
                        <!-- Link to Contact to Book -->
                        <a href="#contact" class="btn btn-book">Book Now</a>
                    </div>
                </article>

                <!-- Stay 3 -->
                <article class="card">
                    <div class="card-img-wrapper">
                        <!-- REPLACE WITH YOUR OWN IMAGE -->
                        <img src="https://picsum.photos/seed/sigiriyarockview/400/300.jpg" alt="Sigiriya Resort" class="card-img">
                    </div>
                    <div class="card-content">
                        <span class="card-meta">Cultural Triangle</span>
                        <h3>Sigiriya Rock Resort</h3>
                        <p style="font-size: 0.9rem; margin: 10px 0; color: var(--text-light);">Luxury tents with a view of the ancient Lion Rock fortress.</p>
                        <!-- Link to Contact to Book -->
                        <a href="#contact" class="btn btn-book">Book Now</a>
                    </div>
                </article>
            </div>
        </div>
    </section>

    <!-- Experiences Section -->
    <section id="experiences" class="section-padding" style="background-color: var(--bg-light);">
        <div class="container reveal">
            <div class="text-center">
                <span class="section-subtitle" data-i18n="adventure">Adventure</span>
                <h2 class="section-title" data-i18n="exp_title">Unique Experiences</h2>
            </div>

            <div class="grid-3">
                <div style="background: white; padding: 20px; border-radius: 8px; box-shadow: var(--shadow);">
                    <i class="fas fa-mountain" style="font-size: 2rem; color: var(--accent-color); margin-bottom: 15px;"></i>
                    <h4>Hiking &amp; Trekking</h4>
                    <p style="font-size: 0.9rem;">Explore Adams Peak or Horton Plains with expert guides.</p>
                </div>
                <div style="background: white; padding: 20px; border-radius: 8px; box-shadow: var(--shadow);">
                    <i class="fas fa-utensils" style="font-size: 2rem; color: var(--accent-color); margin-bottom: 15px;"></i>
                    <h4>Culinary Tours</h4>
                    <p style="font-size: 0.9rem;">Taste authentic Sri Lankan rice and curry cooking classes.</p>
                </div>
                <div style="background: white; padding: 20px; border-radius: 8px; box-shadow: var(--shadow);">
                    <i class="fas fa-paw" style="font-size: 2rem; color: var(--accent-color); margin-bottom: 15px;"></i>
                    <h4>Wildlife Safari</h4>
                    <p style="font-size: 0.9rem;">Leopard and elephant safaris in Yala or Wilpattu National Parks.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery" class="section-padding">
        <div class="container reveal">
            <div class="text-center">
                <h2 class="section-title">Visual Journey</h2>
                <p style="margin-bottom: 30px;">Snapshots of the paradise awaiting you.</p>
            </div>
            
            <div class="gallery-grid">
                <!-- REPLACE WITH YOUR OWN GALLERY IMAGES BELOW -->
                <div class="gallery-item"><img src="https://picsum.photos/seed/srilanka1/600/400.jpg" alt="Gallery Image 1"></div>
                <div class="gallery-item"><img src="https://picsum.photos/seed/srilanka2/600/400.jpg" alt="Gallery Image 2"></div>
                <div class="gallery-item"><img src="https://picsum.photos/seed/srilanka3/600/400.jpg" alt="Gallery Image 3"></div>
                <div class="gallery-item"><img src="https://picsum.photos/seed/srilanka4/600/400.jpg" alt="Gallery Image 4"></div>
                <div class="gallery-item"><img src="https://picsum.photos/seed/srilanka5/600/400.jpg" alt="Gallery Image 5"></div>
                <div class="gallery-item"><img src="https://picsum.photos/seed/srilanka6/600/400.jpg" alt="Gallery Image 6"></div>
                <div class="gallery-item"><img src="https://picsum.photos/seed/srilanka7/600/400.jpg" alt="Gallery Image 7"></div>
                <div class="gallery-item"><img src="https://picsum.photos/seed/srilanka8/600/400.jpg" alt="Gallery Image 8"></div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section id="testimonials" class="section-padding">
        <div class="container reveal">
            <div class="text-center">
                <h2 class="section-title">What Travelers Say</h2>
            </div>
            <div class="grid-3" style="margin-top: 40px;">
                <div class="testimonial-card">
                    <div class="stars"><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></div>
                    <p>"The best trip of my life! Ceylon Island Vibe organized everything perfectly. The tea trails were magical."</p>
                    <h4 style="margin-top: 20px; color: var(--white);">- Sarah J.</h4>
                </div>
                <div class="testimonial-card">
                    <div class="stars"><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></div>
                    <p>"Professional, friendly, and authentic. We saw leopards in Yala and stayed in the most amazing hotels."</p>
                    <h4 style="margin-top: 20px; color: var(--white);">- Mark &amp; Lisa</h4>
                </div>
                <div class="testimonial-card">
                    <div class="stars"><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star-half-alt"></i></div>
                    <p>"Highly recommended for anyone wanting to see the real Sri Lanka without any hassle."</p>
                    <h4 style="margin-top: 20px; color: var(--white);">- Elena R.</h4>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section-padding">
        <div class="container reveal">
            <div class="text-center">
                <span class="section-subtitle" data-i18n="get_in_touch">Get in Touch</span>
                <h2 class="section-title" data-i18n="contact_title">Plan Your Trip</h2>
                <p style="margin-bottom: 40px; max-width: 600px; margin-left: auto; margin-right: auto;">Fill out the form below and our travel experts will craft a personalized itinerary for you.</p>
            </div>

            <div class="contact-wrapper">
                <form id="bookingForm">
                    <div class="form-group">
                        <label for="name" data-i18n="form_name">Full Name</label>
                        <input type="text" id="name" class="form-control" required="">
                    </div>
                    <div class="form-group">
                        <label for="email" data-i18n="form_email">Email Address</label>
                        <input type="email" id="email" class="form-control" required="">
                    </div>
                    <div class="form-group">
                        <label for="interest" data-i18n="form_interest">Interested In</label>
                        <select id="interest" class="form-control">
                            <option value="Stays">Luxury Stays</option>
                            <option value="Tours">Cultural Tours</option>
                            <option value="Safari">Safari Adventures</option>
                            <option value="Other">Other</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="message" data-i18n="form_message">Message</label>
                        <textarea id="message" rows="4" class="form-control"></textarea>
                    </div>
                    <button type="submit" class="btn btn-primary" style="width: 100%;" data-i18n="form_submit">Send Inquiry</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-grid">
                <div>
                    <a href="#" class="footer-logo">Ceylon Island Vibe</a>
                    <p>Your gateway to the authentic Sri Lankan experience. Luxury, adventure, and memories await.</p>
                </div>
                <div>
                    <h4 style="color: var(--white);">Quick Links</h4>
                    <ul class="footer-links">
                        <li><a href="#hero">Home</a></li>
                        <li><a href="#stays">Stays</a></li>
                        <li><a href="#experiences">Experiences</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                <div>
                    <h4 style="color: var(--white);">Contact Us</h4>
                    <ul class="footer-links">
                        <li><i class="fas fa-phone"></i>&nbsp;&nbsp;+971 50 933 91 67&nbsp;</li>
                        <li><i class="fas fa-envelope"></i> hello@ceylonislandvibe.com</li>
                        <li><i class="fas fa-map-marker-alt"></i> Colombo, Sri Lanka</li>
                    </ul>
                    <div class="social-icons" style="margin-top: 20px;">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-tripadvisor"></i></a>
                    </div>
                </div>
            </div>
            <div class="copyright">
                <p>© 2023 Ceylon Island Vibe. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Sticky WhatsApp Button -->
    <!-- CHANGE THE NUMBER BELOW (Replace 94770000000 with your real number) -->
    <a href="https://wa.me/94770000000" class="whatsapp-float" target="_blank" aria-label="Chat on WhatsApp">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- Lightbox Modal -->
    <div class="lightbox" id="lightbox">
        <span class="lightbox-close">×</span>
        <img src="" alt="Full view" class="lightbox-img" id="lightbox-img">
    </div>

    <!-- JavaScript -->
    <script>
        // 1. Sticky Header Effect
        window.addEventListener('scroll', function() {
            const header = document.getElementById('header');
            header.classList.toggle('scrolled', window.scrollY > 50);
        });

        // 2. Mobile Menu Toggle
        const hamburger = document.getElementById('hamburger');
        const navMenu = document.getElementById('nav-menu');
        const navLinks = document.querySelectorAll('.nav-link');

        hamburger.addEventListener('click', () => {
            navMenu.classList.toggle('active');
            hamburger.classList.toggle('toggle');
        });

        // Close menu when link is clicked
        navLinks.forEach(link => {
            link.addEventListener('click', () => {
                navMenu.classList.remove('active');
            });
        });

        // 3. Gallery Lightbox
        const galleryItems = document.querySelectorAll('.gallery-item img');
        const lightbox = document.getElementById('lightbox');
        const lightboxImg = document.getElementById('lightbox-img');
        const lightboxClose = document.querySelector('.lightbox-close');

        galleryItems.forEach(item => {
            item.addEventListener('click', () => {
                lightbox.classList.add('active');
                lightboxImg.src = item.src;
            });
        });

        lightboxClose.addEventListener('click', () => {
            lightbox.classList.remove('active');
        });

        lightbox.addEventListener('click', (e) => {
            if(e.target !== lightboxImg) {
                lightbox.classList.remove('active');
            }
        });

        // 4. Scroll Reveal Animations
        const revealElements = document.querySelectorAll('.reveal');

        function reveal() {
            var windowHeight = window.innerHeight;
            var elementVisible = 150;

            for (var i = 0; i < revealElements.length; i++) {
                var elementTop = revealElements[i].getBoundingClientRect().top;
                if (elementTop < windowHeight - elementVisible) {
                    revealElements[i].classList.add("active");
                }
            }
        }

        window.addEventListener("scroll", reveal);
        // Trigger once on load
        reveal();

        // 5. Form Validation & Custom Toast
        const form = document.getElementById('bookingForm');
        
        form.addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Simple validation check
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;

            if(name && email) {
                showToast();
                form.reset();
            }
        });

        function showToast() {
            var x = document.getElementById("toast");
            x.className = "show";
            setTimeout(function(){ x.className = x.className.replace("show", ""); }, 3000);
        }

        // 6. Multi-Language Toggle System
        const translations = {
            en: {
                home: "Home",
                stays: "Stays",
                experiences: "Experiences",
                gallery: "Gallery",
                contact: "Contact",
                hero_title: "Discover the Soul of Sri Lanka",
                hero_subtitle: "From golden beaches to misty tea plantations, experience the journey of a lifetime.",
                explore_stays: "Explore Stays",
                plan_adventure: "Plan Your Adventure",
                our_story: "Our Story",
                about_title: "Authentic Ceylonese Hospitality",
                accommodation: "Accommodation",
                stays_title: "Curated Luxury Stays",
                adventure: "Adventure",
                exp_title: "Unique Experiences",
                get_in_touch: "Get in Touch",
                contact_title: "Plan Your Trip",
                form_name: "Full Name",
                form_email: "Email Address",
                form_interest: "Interested In",
                form_message: "Message",
                form_submit: "Send Inquiry"
            },
            de: {
                home: "Startseite",
                stays: "Unterkünfte",
                experiences: "Erlebnisse",
                gallery: "Galerie",
                contact: "Kontakt",
                hero_title: "Entdecken Sie die Seele Sri Lankas",
                hero_subtitle: "Von goldenen Stränden bis zu nebelverhangenen Teeplantagen. Erleben Sie die Reise Ihres Lebens.",
                explore_stays: "Unterkünfte",
                plan_adventure: "Abenteuer planen",
                our_story: "Unsere Geschichte",
                about_title: "Authentische singhalesische Gastfreundschaft",
                accommodation: "Unterkunft",
                stays_title: "Ausgewählte Luxusunterkünfte",
                adventure: "Abenteuer",
                exp_title: "Einzigartige Erlebnisse",
                get_in_touch: "Kontaktieren Sie uns",
                contact_title: "Planen Sie Ihre Reise",
                form_name: "Vollständiger Name",
                form_email: "E-Mail-Adresse",
                form_interest: "Interesse an",
                form_message: "Nachricht",
                form_submit: "Anfrage senden"
            },
            fr: {
                home: "Accueil",
                stays: "Séjours",
                experiences: "Expériences",
                gallery: "Galerie",
                contact: "Contact",
                hero_title: "Découvrez l'âme du Sri Lanka",
                hero_subtitle: "Des plages dorées aux plantations de thé brumeuses, vivez le voyage d'une vie.",
                explore_stays: "Explorer les Séjours",
                plan_adventure: "Planifier l'Aventure",
                our_story: "Notre Histoire",
                about_title: "Hospitalité cingalaise authentique",
                accommodation: "Hébergement",
                stays_title: "Séjours de luxe sélectionnés",
                adventure: "Aventure",
                exp_title: "Expériences uniques",
                get_in_touch: "Entrer en contact",
                contact_title: "Planifiez votre voyage",
                form_name: "Nom complet",
                form_email: "Adresse e-mail",
                form_interest: "Intéressé par",
                form_message: "Message",
                form_submit: "Envoyer la demande"
            }
        };

        function setLanguage(lang) {
            const elements = document.querySelectorAll('[data-i18n]');
            
            // Update active state on buttons
            document.querySelectorAll('.lang-btn').forEach(btn => btn.classList.remove('active'));
            event.target.classList.add('active');

            // Update text content
            elements.forEach(el => {
                const key = el.getAttribute('data-i18n');
                if(translations[lang][key]) {
                    el.innerText = translations[lang][key];
                }
            });
        }
    </script>

</body></html>
