<!DOCTYPE html>
<html lang="en">
<head>
  <!-- =========================================
       ✅ SEO & PERFORMANCE METADATA
       ========================================= -->
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  
  <title>Ceylon Island Vibe | Sri Lanka Stays & Experiences</title>
  <meta name="description" content="Discover authentic stays, cultural experiences, and island adventures in Sri Lanka with Ceylon Island Vibe." />
  <meta name="theme-color" content="#064e3b">

  <!-- Open Graph / Facebook -->
  <meta property="og:type" content="website">
  <meta property="og:url" content="https://www.ceylonislandvibe.com/">
  <meta property="og:title" content="Ceylon Island Vibe | Sri Lanka Stays & Experiences">
  <meta property="og:description" content="Discover authentic stays, cultural experiences, and island adventures in Sri Lanka.">
  <meta property="og:image" content="https://z-cdn-media.chatglm.cn/files/451c90fd-bbbf-43b2-9278-6400415cc880.jpeg?auth_key=1868459913-d713f1e5262e4ae9bd6e149179e3ab40-0-a4bcda2e841232ee1d768bfa0083c381">

  <!-- =========================================
       ✅ FONTS (Optimized)
       ========================================= -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&display=swap" rel="stylesheet">

  <!-- =========================================
       ✅ ICONS
       ========================================= -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <!-- =========================================
       ✅ ENHANCED STYLES
       ========================================= -->
  <style>
    /* =========================================
       CSS VARIABLES & RESET
       ========================================= */
    :root {
      --primary-color: #064e3b;
      --primary-dark: #022c22;
      --primary-light: #10b981;
      --accent-color: #d97706;
      --accent-hover: #b45309;
      
      --text-dark: #1f2937;
      --text-light: #6b7280;
      --text-white: #ffffff;
      
      --bg-light: #f9fafb;
      --bg-white: #ffffff;
      --bg-dark: #111827;

      --spacing-xs: 0.5rem;
      --spacing-sm: 1rem;
      --spacing-md: 2rem;
      --spacing-lg: 4rem;
      --spacing-xl: 6rem;

      --font-main: 'Inter', sans-serif;
      --font-heading: 'Playfair Display', serif;
      --transition-speed: 0.3s;
      --ease-out: cubic-bezier(0.215, 0.61, 0.355, 1);

      --shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
      --shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
      --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
      --shadow-hover: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);

      --radius-sm: 6px;
      --radius-md: 12px;
      --radius-full: 9999px;
      --header-height: 80px;
    }

    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }
    html { scroll-behavior: smooth; font-size: 16px; }
    
    body {
      font-family: var(--font-main);
      color: var(--text-dark);
      line-height: 1.7;
      overflow-x: hidden;
      background-color: var(--bg-white);
      -webkit-font-smoothing: antialiased;
    }

    :focus-visible {
      outline: 3px solid var(--accent-color);
      outline-offset: 2px;
    }

    h1,h2,h3,h4,h5,h6 {
      font-family: var(--font-heading);
      color: var(--primary-color);
      line-height: 1.2;
      margin-bottom: var(--spacing-sm);
    }

    a { text-decoration: none; color: inherit; transition: color var(--transition-speed) ease; }
    ul { list-style: none; }
    img { max-width: 100%; height: auto; display: block; }

    .container { 
      width: 90%; 
      max-width: 1280px; 
      margin: 0 auto; 
      padding: 0 var(--spacing-sm); 
    }
    
    .section-padding { padding: var(--spacing-xl) 0; }
    .text-center { text-align: center; }

    .section-title {
      font-size: 2.5rem;
      margin-bottom: var(--spacing-xs);
      position: relative;
      display: inline-block;
    }

    .section-subtitle {
      color: var(--accent-color);
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 2px;
      font-size: 0.85rem;
      display: block;
      margin-bottom: var(--spacing-sm);
    }

    /* =========================================
       COMPONENTS: BUTTONS
       ========================================= */
    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 12px 32px;
      border-radius: var(--radius-full);
      font-weight: 600;
      cursor: pointer;
      border: 2px solid transparent;
      transition: all var(--transition-speed) var(--ease-out);
      letter-spacing: 0.5px;
    }

    .btn-primary { 
      background-color: var(--primary-color); 
      color: var(--text-white); 
      box-shadow: var(--shadow-md);
    }
    .btn-primary:hover { 
      background-color: var(--primary-dark); 
      transform: translateY(-2px); 
      box-shadow: var(--shadow-hover);
    }

    .btn-outline {
      border-color: var(--text-white);
      color: var(--text-white);
      background: rgba(255,255,255,0.1);
      backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
    }
    .btn-outline:hover { 
      background-color: var(--text-white); 
      color: var(--primary-color); 
      transform: translateY(-2px);
    }

    .btn-book {
      background-color: var(--accent-color);
      color: var(--text-white);
      font-size: 0.9rem;
      padding: 10px 24px;
      box-shadow: var(--shadow-sm);
      border-radius: var(--radius-sm);
    }
    .btn-book:hover { background-color: var(--accent-hover); transform: translateY(-1px); }

    /* =========================================
       HEADER & NAVIGATION
       ========================================= */
    header {
      position: fixed;
      top: 0; left: 0; width: 100%;
      z-index: 1000;
      padding: 20px 0;
      transition: all 0.4s var(--ease-out);
    }

    header.scrolled { 
      background-color: rgba(255, 255, 255, 0.95);
      backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
      box-shadow: var(--shadow-sm); 
      padding: 15px 0; 
    }
    
    header.scrolled .logo { color: var(--primary-color); }
    header.scrolled .nav-link { color: var(--text-dark); }
    header.scrolled .hamburger div { background-color: var(--text-dark); }

    .nav-container { display: flex; justify-content: space-between; align-items: center; }
    
    .logo {
      font-family: var(--font-heading);
      font-size: 1.8rem;
      font-weight: 700;
      color: var(--text-white);
      letter-spacing: 1px;
      z-index: 1002;
    }

    .nav-menu { display: flex; align-items: center; gap: 35px; }
    
    .nav-link {
      color: var(--text-white);
      font-weight: 500;
      font-size: 0.95rem;
      position: relative;
      padding: 5px 0;
    }
    .nav-link::after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      bottom: 0;
      left: 0;
      background-color: var(--accent-color);
      transition: width var(--transition-speed) var(--ease-out);
    }
    .nav-link:hover::after { width: 100%; }

    .lang-toggle { display: flex; gap: 10px; margin-left: 20px; border-left: 1px solid rgba(255,255,255,0.3); padding-left: 20px; }
    .lang-btn {
      background: none;
      border: none;
      color: var(--text-white);
      font-size: 0.8rem;
      font-weight: bold;
      cursor: pointer;
      opacity: 0.6;
      transition: opacity 0.2s;
    }
    header.scrolled .lang-btn { color: var(--text-dark); }
    .lang-btn.active { opacity: 1; }
    .lang-btn:hover { opacity: 1; }

    .hamburger { display: none; cursor: pointer; z-index: 1002; }
    .hamburger div { 
      width: 25px; height: 3px; 
      background-color: var(--text-white); 
      margin: 5px 0; 
      transition: all 0.3s var(--ease-out); 
      border-radius: 2px;
    }

    /* =========================================
       HERO SECTION
       ========================================= */
    #hero {
      height: 100vh;
      background: linear-gradient(135deg, rgba(0,0,0,0.4) 0%, rgba(0,0,0,0.2) 100%),
        url('https://z-cdn-media.chatglm.cn/files/451c90fd-bbbf-43b2-9278-6400415cc880.jpeg?auth_key=1868459913-d713f1e5262e4ae9bd6e149179e3ab40-0-a4bcda2e841232ee1d768bfa0083c381') center/cover no-repeat;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: var(--text-white);
      position: relative;
    }

    #hero::before {
      content: '';
      position: absolute;
      top: 0; left: 0; width: 100%; height: 100%;
      background: inherit;
      z-index: -1;
      will-change: transform;
      animation: zoomEffect 25s infinite alternate ease-in-out;
    }

    .hero-content { max-width: 800px; padding: 20px; z-index: 1; }
    .hero-title { 
      font-size: 3.5rem; 
      margin-bottom: 20px; 
      color: var(--text-white); /* Title changed to white */
      opacity: 0; 
      transform: translateY(30px); 
      animation: fadeUp 1s var(--ease-out) forwards 0.5s; 
      text-shadow: 0 2px 10px rgba(0,0,0,0.3); 
    }
    .hero-text { font-size: 1.25rem; margin-bottom: 35px; opacity: 0; transform: translateY(30px); animation: fadeUp 1s var(--ease-out) forwards 0.8s; text-shadow: 0 1px 5px rgba(0,0,0,0.3); }
    .hero-btns { opacity: 0; animation: fadeUp 1s var(--ease-out) forwards 1.1s; display: flex; gap: 15px; justify-content: center; }

    /* =========================================
       CARDS & GRIDS
       ========================================= */
    .grid-3 { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; margin-top: 40px; }
    .grid-4 { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 20px; margin-top: 40px; }

    .card {
      background: var(--bg-white);
      border-radius: var(--radius-md);
      overflow: hidden;
      box-shadow: var(--shadow-md);
      transition: all 0.4s var(--ease-out);
      position: relative;
      display: flex;
      flex-direction: column;
      height: 100%;
    }
    .card:hover { transform: translateY(-8px); box-shadow: var(--shadow-hover); }

    .card-img-wrapper { overflow: hidden; height: 260px; position: relative; }
    .card-img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.6s var(--ease-out); }
    .card:hover .card-img { transform: scale(1.08); }

    .card-content { padding: 25px; flex-grow: 1; display: flex; flex-direction: column; justify-content: space-between; }
    .card-meta { font-size: 0.85rem; color: var(--accent-color); margin-bottom: 8px; display: flex; align-items: center; gap: 5px; font-weight: 600; }
    .card-title { font-size: 1.4rem; margin-bottom: 10px; }
    .card-desc { color: var(--text-light); font-size: 0.95rem; margin-bottom: 20px; }

    /* =========================================
       SECTIONS (About, Gallery, Testimonials)
       ========================================= */
    #about { background-color: var(--bg-light); }
    .about-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 60px; align-items: center; }
    
    .about-img-wrapper {
      border-radius: var(--radius-md);
      overflow: hidden;
      box-shadow: var(--shadow-lg);
      position: relative;
    }
    .about-img-wrapper::before {
      content: ''; position: absolute; top:0; left:0; width:100%; height:100%;
      background: rgba(6,78,59,0.1); z-index: 1;
    }
    .about-img-wrapper:hover::before { opacity: 0; }

    .gallery-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; }
    .gallery-item { 
      cursor: pointer; 
      overflow: hidden; 
      border-radius: var(--radius-sm); 
      height: 300px; 
      position: relative;
    }
    .gallery-item::after {
      content: '\f00e';
      font-family: 'Font Awesome 6 Free';
      font-weight: 900;
      position: absolute;
      top: 50%; left: 50%;
      transform: translate(-50%, -50%) scale(0.5);
      color: #fff;
      font-size: 2rem;
      opacity: 0;
      transition: 0.3s ease;
    }
    .gallery-item img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.5s ease; }
    .gallery-item:hover img { transform: scale(1.1); filter: brightness(0.7); }
    .gallery-item:hover::after { opacity: 1; transform: translate(-50%, -50%) scale(1); }

    #testimonials { 
      background-color: var(--primary-color); 
      color: var(--text-white); 
      background-image: radial-gradient(circle at top right, #047857 0%, transparent 40%),
                        radial-gradient(circle at bottom left, #065f46 0%, transparent 40%);
    }
    #testimonials .section-title, #testimonials h2 { color: var(--text-white); }

    .testimonial-card {
      background: rgba(255,255,255,0.05);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      padding: 40px;
      border-radius: var(--radius-md);
      border: 1px solid rgba(255,255,255,0.1);
      transition: var(--transition-speed);
    }
    .testimonial-card:hover { background: rgba(255,255,255,0.1); }
    .stars { color: var(--accent-color); margin-bottom: 15px; letter-spacing: 2px; }

    /* =========================================
       FORMS
       ========================================= */
    .contact-wrapper {
      background: var(--bg-white);
      padding: 50px;
      border-radius: var(--radius-md);
      box-shadow: var(--shadow-lg);
      max-width: 650px;
      margin: 0 auto;
    }
    .form-group { margin-bottom: 25px; }
    .form-group label { display: block; margin-bottom: 10px; font-weight: 500; color: var(--text-dark); }
    .form-control {
      width: 100%;
      padding: 14px 16px;
      border: 1px solid #e5e7eb;
      border-radius: var(--radius-sm);
      font-family: inherit;
      transition: var(--transition-speed);
      background-color: #f9fafb;
    }
    .form-control:focus { 
      outline: none; 
      border-color: var(--primary-color); 
      background-color: #fff;
      box-shadow: 0 0 0 4px rgba(6, 78, 59, 0.1); 
    }

    /* =========================================
       FOOTER
       ========================================= -->
    footer { background-color: var(--bg-dark); color: #9ca3af; padding: 80px 0 30px; }
    .footer-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 50px; margin-bottom: 50px; }
    .footer-logo { color: var(--text-white); font-family: var(--font-heading); font-size: 1.6rem; margin-bottom: 20px; display: inline-block; }
    .footer-links li { margin-bottom: 12px; }
    .footer-links a { color: #9ca3af; transition: color 0.2s; }
    .footer-links a:hover { color: var(--accent-color); padding-left: 5px; }
    
    .social-icons { display: flex; gap: 15px; }
    .social-icons a {
      width: 44px; height: 44px;
      background: rgba(255,255,255,0.05);
      display: flex; align-items: center; justify-content: center;
      border-radius: 50%;
      transition: all 0.3s ease;
      color: #fff;
    }
    .social-icons a:hover { background: var(--primary-color); transform: translateY(-3px); box-shadow: 0 5px 15px rgba(0,0,0,0.3); }

    .copyright {
      text-align: center;
      padding-top: 30px;
      border-top: 1px solid rgba(255,255,255,0.08);
      font-size: 0.9rem;
    }

    /* =========================================
       INTERACTIVE ELEMENTS
       ========================================= */
    .lightbox {
      position: fixed;
      top: 0; left: 0; width: 100%; height: 100%;
      background: rgba(0,0,0,0.95);
      z-index: 2000;
      display: none;
      justify-content: center;
      align-items: center;
      padding: 20px;
      backdrop-filter: blur(5px);
    }
    .lightbox.active { display: flex; animation: fadeIn 0.3s ease; }
    .lightbox-img { max-width: 95%; max-height: 90vh; border-radius: 4px; box-shadow: 0 0 40px rgba(0,0,0,0.5); }
    .lightbox-close { position: absolute; top: 30px; right: 30px; color: #fff; font-size: 2.5rem; cursor: pointer; transition: color 0.2s; }
    .lightbox-close:hover { color: var(--accent-color); }

    #toast {
      visibility: hidden;
      min-width: 280px;
      background-color: var(--text-dark);
      color: #fff;
      text-align: center;
      border-radius: 8px;
      padding: 16px;
      position: fixed;
      z-index: 3000;
      left: 50%;
      bottom: 30px;
      transform: translateX(-50%) translateY(20px);
      font-size: 1rem;
      box-shadow: var(--shadow-lg);
      opacity: 0;
      transition: all 0.4s var(--ease-out);
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 10px;
    }
    #toast.show { visibility: visible; transform: translateX(-50%) translateY(0); opacity: 1; }
    #toast i { color: var(--accent-color); }

    .whatsapp-float {
      position: fixed;
      width: 65px; height: 65px;
      bottom: 40px; right: 40px;
      background-color: #25d366;
      color: #FFF;
      border-radius: 50%;
      text-align: center;
      font-size: 32px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
      z-index: 999;
      display: flex;
      align-items: center;
      justify-content: center;
      transition: all 0.3s var(--ease-out);
    }
    .whatsapp-float:hover { background-color: #128c7e; transform: scale(1.1) rotate(10deg); }

    ::-webkit-scrollbar { width: 10px; }
    ::-webkit-scrollbar-track { background: #f1f1f1; }
    ::-webkit-scrollbar-thumb { background: #cbd5e1; border-radius: 5px; }
    ::-webkit-scrollbar-thumb:hover { background: var(--primary-color); }

    @keyframes zoomEffect { 0% { transform: scale(1); } 100% { transform: scale(1.15); } }
    @keyframes fadeUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }
    @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

    .reveal { position: relative; transform: translateY(50px); opacity: 0; transition: 1s all var(--ease-out); }
    .reveal.active { transform: translateY(0); opacity: 1; }

    @media screen and (max-width: 900px) {
      .hero-title { font-size: 2.8rem; }
      .about-grid { grid-template-columns: 1fr; }
    }

    @media screen and (max-width: 768px) {
      .hamburger { display: block; }
      .nav-menu {
        position: fixed; top: 0; right: -100%;
        width: 80%; max-width: 300px; height: 100vh;
        background-color: var(--bg-white);
        flex-direction: column; justify-content: center;
        box-shadow: -10px 0 30px rgba(0,0,0,0.1);
        transition: 0.4s cubic-bezier(0.77, 0, 0.175, 1);
      }
      .nav-menu.active { right: 0; }
      .nav-link { color: var(--text-dark); font-size: 1.2rem; }
      .lang-toggle { color: var(--text-dark); margin: 30px 0; border-left: none; border-top: 1px solid #eee; padding-left: 0; padding-top: 20px; width: 100%; justify-content: center; }
      .hero-title { font-size: 2.2rem; }
      .hero-btns { flex-direction: column; width: 100%; }
      .btn { width: 100%; }
      .whatsapp-float { width: 55px; height: 55px; font-size: 28px; bottom: 20px; right: 20px; }
      .contact-wrapper { padding: 30px 20px; }
    }

    @media (prefers-reduced-motion: reduce) {
      html { scroll-behavior: auto; }
      *, *::before, *::after {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
        scroll-behavior: auto !important;
      }
      #hero::before { animation: none; }
    }
  </style>
</head>
<body>

  <!-- =========================================
       HEADER
       ========================================= -->
  <header id="header">
    <div class="container nav-container">
      <a href="#" class="logo">Ceylon Island Vibe</a>
      
      <nav>
        <ul class="nav-menu">
          <li><a href="#hero" class="nav-link">Home</a></li>
          <li><a href="#about" class="nav-link">About</a></li>
          <li><a href="#experiences" class="nav-link">Experiences</a></li>
          <li><a href="#gallery" class="nav-link">Gallery</a></li>
          <li><a href="#contact" class="nav-link">Contact</a></li>
          
          <div class="lang-toggle">
            <button class="lang-btn active">EN</button>
            <button class="lang-btn">SI</button>
          </div>
        </ul>
      </nav>

      <div class="hamburger">
        <div class="line1"></div>
        <div class="line2"></div>
        <div class="line3"></div>
      </div>
    </div>
  </header>

  <!-- =========================================
       HERO SECTION
       ========================================= -->
  <section id="hero">
    <div class="hero-content text-center">
      <h1 class="hero-title">Experience the Soul of Sri Lanka</h1>
      <p class="hero-text">From the misty mountains of Ella to the golden sands of the south coast. Discover your perfect island vibe.</p>
      <div class="hero-btns">
        <a href="#experiences" class="btn btn-primary">Explore Experiences</a>
        <a href="#contact" class="btn btn-outline">Plan Your Trip</a>
      </div>
    </div>
  </section>

  <!-- =========================================
       ABOUT SECTION
       ========================================= -->
  <section id="about" class="section-padding">
    <div class="container">
      <div class="about-grid">
        <div class="about-text reveal">
          <span class="section-subtitle">Our Story</span>
          <h2 class="section-title">Authentic Island Hospitality</h2>
          <p style="margin-bottom: 20px; color: var(--text-light);">
            At Ceylon Island Vibe, we don't just offer a place to stay; we offer a gateway to the heart of Sri Lanka. Whether you are seeking the adrenaline of surfing on Arugam Bay or the serene tranquility of tea country, we curate experiences that connect you with nature and culture.
          </p>
          <p style="margin-bottom: 30px; color: var(--text-light);">
            Our hand-picked locations, from eco-friendly bamboo structures to luxury lounges, ensure that your stay is comfortable, sustainable, and unforgettable.
          </p>
          <a href="#contact" class="btn btn-primary">Learn More</a>
        </div>
        
        <div class="about-img-wrapper reveal">
          <!-- Image 7: Mountain Landscape -->
          <img src="https://z-cdn-media.chatglm.cn/files/830e70f6-497b-4372-83a5-13f0c1527101.jpeg?auth_key=1868459913-4e29ce4e78074a89a730c34863b8c1b3-0-097c7d2a08b1342065276926655dc89a" alt="Sri Lankan Mountains" class="card-img">
        </div>
      </div>
    </div>
  </section>

  <!-- =========================================
       EXPERIENCES & STAYS
       ========================================= -->
  <section id="experiences" class="section-padding">
    <div class="container">
      <div class="text-center reveal">
        <span class="section-subtitle">Curated For You</span>
        <h2 class="section-title">Stays & Adventures</h2>
        <p style="max-width: 600px; margin: 0 auto; color: var(--text-light);">Discover our selection of unique accommodations and thrilling activities designed for the modern traveler.</p>
      </div>

      <div class="grid-3">
        <!-- Card 1: Surfing -->
        <article class="card reveal">
          <div class="card-img-wrapper">
            <!-- Image 4: Surfing -->
            <img src="https://z-cdn-media.chatglm.cn/files/e941d547-a11b-45ba-94fc-756942ccc7ae.jpeg?auth_key=1868459913-8e05db73e5974ac0997541d886c0698c-0-485bf607188752deffecaefa2b519672" alt="Surfing in Sri Lanka" class="card-img">
          </div>
          <div class="card-content">
            <div>
              <span class="card-meta"><i class="fas fa-water"></i> Adventure</span>
              <h3 class="card-title">Ride the Waves</h3>
              <p class="card-desc">Experience world-class surfing breaks. Perfect for beginners and pros alike looking for the thrill of the ocean.</p>
            </div>
            <a href="#contact" class="btn-book">Book Session</a>
          </div>
        </article>

        <!-- Card 2: Snorkeling -->
        <article class="card reveal">
          <div class="card-img-wrapper">
            <!-- Image 3: Snorkeling -->
            <img src="https://z-cdn-media.chatglm.cn/files/fdae3125-d1fd-41b2-8e9d-b3526c3bd514.jpeg?auth_key=1868459913-d2a2257a8ac04fb3ad2f4adc115c24b8-0-ffdcc66df9a33a2a72d7279bc57a5142" alt="Snorkeling Coral Reefs" class="card-img">
          </div>
          <div class="card-content">
            <div>
              <span class="card-meta"><i class="fas fa-fish"></i> Ocean Life</span>
              <h3 class="card-title">Reef Exploration</h3>
              <p class="card-desc">Dive into crystal clear waters to witness vibrant coral reefs and tropical marine life up close.</p>
            </div>
            <a href="#contact" class="btn-book">Explore</a>
          </div>
        </article>

        <!-- Card 3: Bamboo Dining -->
        <article class="card reveal">
          <div class="card-img-wrapper">
            <!-- Image 2: Bamboo Restaurant -->
            <img src="https://z-cdn-media.chatglm.cn/files/4c7700e8-81a0-44bd-b9f8-a47cced3d2ff.jpeg?auth_key=1868459913-3e5184f4ecb34e24acc7bb43565cb45f-0-5cb85f12c7fc78fa35fe2e57ec3f0653" alt="Bamboo Restaurant" class="card-img">
          </div>
          <div class="card-content">
            <div>
              <span class="card-meta"><i class="fas fa-utensils"></i> Dining</span>
              <h3 class="card-title">Jungle Gastronomy</h3>
              <p class="card-desc">Dine under the stars in our eco-friendly bamboo structure, enjoying local fusion cuisine in a cozy atmosphere.</p>
            </div>
            <a href="#contact" class="btn-book">View Menu</a>
          </div>
        </article>

        <!-- Card 4: Heaven's Gate Ella -->
        <article class="card reveal">
          <div class="card-img-wrapper">
            <!-- Image 6: Heaven's Gate Ella -->
            <img src="https://z-cdn-media.chatglm.cn/files/fefeb10c-19b9-40bd-b38f-00378c37e5bc.jpeg?auth_key=1868459913-b931c8570af84f01a6c8c8157042823f-0-3b8bdf295e55fccafe9bacaf109fe71a" alt="Heaven's Gate Ella Lounge" class="card-img">
          </div>
          <div class="card-content">
            <div>
              <span class="card-meta"><i class="fas fa-couch"></i> Relaxation</span>
              <h3 class="card-title">Heaven's Gate Ella</h3>
              <p class="card-desc">Unwind in our signature lounge in Ella. Sip Ceylon tea while enjoying the cool breeze and mountain views.</p>
            </div>
            <a href="#contact" class="btn-book">Stay Here</a>
          </div>
        </article>
      </div>
    </div>
  </section>

  <!-- =========================================
       GALLERY
       ========================================= -->
  <section id="gallery" class="section-padding">
    <div class="container">
      <div class="text-center reveal" style="margin-bottom: 50px;">
        <span class="section-subtitle">Visual Diary</span>
        <h2 class="section-title">Captured Moments</h2>
      </div>
      
      <div class="gallery-grid">
        <!-- Image 1: Welcome Sign -->
        <div class="gallery-item reveal">
          <img src="https://z-cdn-media.chatglm.cn/files/e58007d7-37a8-49d1-b0ba-a31ebc99dee2.jpeg?auth_key=1868459913-f7b7a97c3ccf41cabd4b3cd6e737ee7e-0-62ff3923efff4ce319c86dedbe532932" alt="Welcome to Sri Lanka Sign">
        </div>

        <!-- Image 5: Beach -->
        <div class="gallery-item reveal">
          <img src="https://z-cdn-media.chatglm.cn/files/451c90fd-bbbf-43b2-9278-6400415cc880.jpeg?auth_key=1868459913-d713f1e5262e4ae9bd6e149179e3ab40-0-a4bcda2e841232ee1d768bfa0083c381" alt="Tropical Beach Sunset">
        </div>

        <!-- Image 2: Bamboo Restaurant -->
        <div class="gallery-item reveal">
          <img src="https://z-cdn-media.chatglm.cn/files/4c7700e8-81a0-44bd-b9f8-a47cced3d2ff.jpeg?auth_key=1868459913-3e5184f4ecb34e24acc7bb43565cb45f-0-5cb85f12c7fc78fa35fe2e57ec3f0653" alt="Night Dining">
        </div>

        <!-- Image 7: Mountains -->
        <div class="gallery-item reveal">
          <img src="https://z-cdn-media.chatglm.cn/files/830e70f6-497b-4372-83a5-13f0c1527101.jpeg?auth_key=1868459913-4e29ce4e78074a89a730c34863b8c1b3-0-097c7d2a08b1342065276926655dc89a" alt="Hill Country View">
        </div>

        <!-- Image 6: Interior -->
        <div class="gallery-item reveal">
          <img src="https://z-cdn-media.chatglm.cn/files/fefeb10c-19b9-40bd-b38f-00378c37e5bc.jpeg?auth_key=1868459913-b931c8570af84f01a6c8c8157042823f-0-3b8bdf295e55fccafe9bacaf109fe71a" alt="Cozy Interior">
        </div>

        <!-- Image 3: Snorkeling -->
        <div class="gallery-item reveal">
          <img src="https://z-cdn-media.chatglm.cn/files/fdae3125-d1fd-41b2-8e9d-b3526c3bd514.jpeg?auth_key=1868459913-d2a2257a8ac04fb3ad2f4adc115c24b8-0-ffdcc66df9a33a2a72d7279bc57a5142" alt="Underwater Life">
        </div>
      </div>
    </div>
  </section>

  <!-- =========================================
       TESTIMONIALS
       ========================================= -->
  <section id="testimonials" class="section-padding">
    <div class="container">
      <div class="text-center" style="margin-bottom: 50px;">
        <span class="section-subtitle" style="color: #fff;">Guest Love</span>
        <h2 class="section-title">What They Say</h2>
      </div>
      
      <div class="grid-3">
        <div class="testimonial-card reveal">
          <div class="stars"><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></div>
          <p>"The bamboo restaurant was the highlight of our trip. The food, the atmosphere, and the staff were absolutely incredible."</p>
          <h4 style="margin-top: 20px; margin-bottom: 0;">Sarah Jenkins</h4>
          <small style="opacity: 0.7;">United Kingdom</small>
        </div>
        
        <div class="testimonial-card reveal">
          <div class="stars"><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></div>
          <p>"Surfing lessons were professional and safe. We saw so many fish while snorkeling. A true paradise experience."</p>
          <h4 style="margin-top: 20px; margin-bottom: 0;">Mark Thompson</h4>
          <small style="opacity: 0.7;">Australia</small>
        </div>
        
        <div class="testimonial-card reveal">
          <div class="stars"><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star-half-alt"></i></div>
          <p>"Heaven's Gate Ella lives up to its name. The view is breathtaking and the tea service was perfect."</p>
          <h4 style="margin-top: 20px; margin-bottom: 0;">Chen Wei</h4>
          <small style="opacity: 0.7;">Singapore</small>
        </div>
      </div>
    </div>
  </section>

  <!-- =========================================
       CONTACT
       ========================================= -->
  <section id="contact" class="section-padding" style="background-color: var(--bg-light);">
    <div class="container">
      <div class="text-center reveal" style="margin-bottom: 50px;">
        <span class="section-subtitle">Get in Touch</span>
        <h2 class="section-title">Start Your Journey</h2>
      </div>

      <div class="contact-wrapper reveal">
        <form id="bookingForm">
          <div class="form-group">
            <label for="name">Full Name</label>
            <input type="text" id="name" class="form-control" placeholder="Enter your name" required>
          </div>
          <div class="form-group">
            <label for="email">Email Address</label>
            <input type="email" id="email" class="form-control" placeholder="Enter your email" required>
          </div>
          <div class="form-group">
            <label for="interest">Interested In</label>
            <select id="interest" class="form-control">
              <option>General Inquiry</option>
              <option>Surfing Lessons</option>
              <option>Bamboo Dining</option>
              <option>Accommodation (Ella)</option>
            </select>
          </div>
          <div class="form-group">
            <label for="message">Message</label>
            <textarea id="message" rows="5" class="form-control" placeholder="Tell us about your travel plans..." required></textarea>
          </div>
          <button type="submit" class="btn btn-primary" style="width: 100%;">Send Message</button>
        </form>
      </div>
    </div>
  </section>

  <!-- =========================================
       FOOTER
       ========================================= -->
  <footer>
    <div class="container">
      <div class="footer-grid">
        <div>
          <a href="#" class="footer-logo">Ceylon Island Vibe</a>
          <p style="font-size: 0.9rem; line-height: 1.8;">
            Your gateway to the authentic beauty of Sri Lanka. We craft memorable stays and adventures for travelers worldwide.
          </p>
        </div>
        
        <div>
          <h4 style="color: #fff;">Quick Links</h4>
          <ul class="footer-links">
            <li><a href="#hero">Home</a></li>
            <li><a href="#about">About Us</a></li>
            <li><a href="#experiences">Experiences</a></li>
            <li><a href="#gallery">Gallery</a></li>
          </ul>
        </div>
        
        <div>
          <h4 style="color: #fff;">Contact</h4>
          <ul class="footer-links">
            <li><i class="fas fa-map-marker-alt" style="margin-right: 10px;"></i> Ella, Sri Lanka</li>
            <li><i class="fas fa-phone" style="margin-right: 10px;"></i> +971 50 933 91 67</li>
            <li><i class="fas fa-envelope" style="margin-right: 10px;"></i> hello@ceylonvibe.com</li>
          </ul>
          <div class="social-icons" style="margin-top: 20px;">
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
          </div>
        </div>
      </div>
      
      <div class="copyright">
        <p>&copy; 2024 Ceylon Island Vibe. All rights reserved.</p>
      </div>
    </div>
  </footer>

  <!-- =========================================
       UI ELEMENTS (Lightbox, Toast, Whatsapp)
       ========================================= -->
  <div class="lightbox" id="lightbox">
    <span class="lightbox-close">&times;</span>
    <img class="lightbox-img" id="lightbox-img" src="" alt="Full view">
  </div>

  <div id="toast"><i class="fas fa-check-circle"></i> Message Sent Successfully!</div>

  <a href="https://wa.me/971509339167" class="whatsapp-float" target="_blank">
    <i class="fab fa-whatsapp"></i>
  </a>

  <!-- =========================================
       JAVASCRIPT
       ========================================= -->
  <script>
    // Sticky Header Animation
    const header = document.querySelector('header');
    window.addEventListener('scroll', () => {
      if (window.scrollY > 50) {
        header.classList.add('scrolled');
      } else {
        header.classList.remove('scrolled');
      }
    });

    // Mobile Menu Toggle
    const hamburger = document.querySelector('.hamburger');
    const navMenu = document.querySelector('.nav-menu');
    const navLinks = document.querySelectorAll('.nav-link');

    hamburger.addEventListener('click', () => {
      hamburger.classList.toggle('active');
      navMenu.classList.toggle('active');
    });

    // Close mobile menu when a link is clicked
    navLinks.forEach(link => {
      link.addEventListener('click', () => {
        hamburger.classList.remove('active');
        navMenu.classList.remove('active');
      });
    });

    // Lightbox Functionality
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
      if (e.target !== lightboxImg) {
        lightbox.classList.remove('active');
      }
    });

    // Scroll Reveal Animation
    const revealElements = document.querySelectorAll('.reveal');

    const revealOnScroll = () => {
      const windowHeight = window.innerHeight;
      const elementVisible = 150;

      revealElements.forEach((reveal) => {
        const elementTop = reveal.getBoundingClientRect().top;
        if (elementTop < windowHeight - elementVisible) {
          reveal.classList.add('active');
        }
      });
    };

    window.addEventListener('scroll', revealOnScroll);
    // Trigger once on load
    revealOnScroll();

    // Contact Form Toast
    const form = document.getElementById('bookingForm');
    const toast = document.getElementById('toast');

    form.addEventListener('submit', (e) => {
      e.preventDefault();
      // Simulate form submission
      toast.className = "show";
      setTimeout(function(){ toast.className = toast.className.replace("show", ""); }, 3000);
      form.reset();
    });
  </script>
</body>
</html>
