<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>DZ-Tourism | Visit Algeria</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@600;700;900&family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />

  <style>
    :root {
      --gold: #dfa83b;
      --gold-dark: #b8860b;
      --gold-light: #fbe29d;
      --dark-bg: #0d1117;
      --card-bg: #161b22;
      --text-main: #f0f6fc;
      --text-muted: #8b949e;
      --accent: #e67e22;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
      scroll-behavior: smooth;
    }

    body {
      background-color: var(--dark-bg);
      color: var(--text-main);
      overflow-x: hidden;
    }

    /* 1. HERO SECTION WITH DESERT SUNSET */
    .hero {
      position: relative;
      height: 90vh;
      background: linear-gradient(rgba(0, 0, 0, 0.45), rgba(13, 17, 23, 0.95)),
                  url('https://images.unsplash.com/photo-1509316975850-ff9c5deb0cd9?auto=format&fit=crop&w=1920&q=80') center/cover no-repeat;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 0 20px;
    }

    .hero-title {
      font-family: 'Cinzel', serif;
      font-size: 3.8rem;
      font-weight: 900;
      letter-spacing: 2px;
      color: var(--gold);
      text-shadow: 0 0 25px rgba(223, 168, 59, 0.6), 0 4px 10px rgba(0,0,0,0.8);
      margin-bottom: 15px;
      text-transform: uppercase;
    }

    .hero-subtitle {
      font-size: 1.3rem;
      max-width: 700px;
      color: #e6edf3;
      margin-bottom: 30px;
      text-shadow: 0 2px 5px rgba(0,0,0,0.8);
    }

    .btn-gold {
      background: linear-gradient(135deg, var(--gold), var(--gold-dark));
      color: #000;
      font-weight: 700;
      padding: 14px 35px;
      border-radius: 50px;
      text-decoration: none;
      font-size: 1.1rem;
      box-shadow: 0 4px 20px rgba(223, 168, 59, 0.4);
      transition: all 0.3s ease;
    }

    .btn-gold:hover {
      transform: translateY(-3px);
      box-shadow: 0 6px 25px rgba(223, 168, 59, 0.7);
    }

    /* GENERAL SECTION STYLING */
    section {
      padding: 70px 8%;
    }

    .section-header {
      text-align: center;
      margin-bottom: 50px;
    }

    .section-title {
      font-size: 2.3rem;
      color: var(--gold);
      font-family: 'Cinzel', serif;
      letter-spacing: 1px;
      margin-bottom: 10px;
    }

    .section-sub {
      color: var(--text-muted);
      font-size: 1rem;
    }

    /* 2. HOTELS SECTION */
    .hotels-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
    }

    .card {
      background-color: var(--card-bg);
      border-radius: 15px;
      overflow: hidden;
      border: 1px solid #30363d;
      transition: transform 0.3s ease, border-color 0.3s ease;
    }

    .card:hover {
      transform: translateY(-7px);
      border-color: var(--gold);
    }

    .card-img-wrap {
      position: relative;
      height: 200px;
    }

    .card-img-wrap img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .badge-price {
      position: absolute;
      top: 15px;
      right: 15px;
      background: rgba(0,0,0,0.75);
      backdrop-filter: blur(5px);
      color: var(--gold);
      padding: 6px 14px;
      border-radius: 20px;
      font-weight: 700;
      font-size: 0.9rem;
      border: 1px solid var(--gold);
    }

    .card-content {
      padding: 20px;
    }

    .card-content h3 {
      font-size: 1.3rem;
      margin-bottom: 6px;
    }

    .card-location {
      color: var(--text-muted);
      font-size: 0.9rem;
      margin-bottom: 12px;
      display: flex;
      align-items: center;
      gap: 6px;
    }

    .rating {
      color: #ffd700;
      margin-bottom: 15px;
      font-size: 0.95rem;
    }

    .btn-book {
      display: block;
      width: 100%;
      text-align: center;
      background: transparent;
      border: 1px solid var(--gold);
      color: var(--gold);
      padding: 10px 0;
      border-radius: 8px;
      font-weight: 600;
      text-decoration: none;
      transition: all 0.3s;
    }

    .btn-book:hover {
      background: var(--gold);
      color: #000;
    }

    /* 3. AGENCIES SECTION */
    .agencies-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 25px;
    }

    .agency-card {
      background: #11161d;
      border: 1px solid #21262d;
      border-radius: 12px;
      padding: 25px;
      text-align: center;
      transition: 0.3s;
    }

    .agency-card:hover {
      border-color: var(--accent);
      box-shadow: 0 5px 20px rgba(230, 126, 34, 0.2);
    }

    .agency-icon {
      font-size: 2.5rem;
      color: var(--gold);
      margin-bottom: 15px;
    }

    .agency-card h3 {
      margin-bottom: 10px;
      font-size: 1.2rem;
    }

    .agency-card p {
      color: var(--text-muted);
      font-size: 0.9rem;
      margin-bottom: 15px;
    }

    /* 4. ANNABA SPECIAL HIGHLIGHT */
    .annaba-showcase {
      background: linear-gradient(180deg, #0d1117 0%, #151b23 100%);
      border-radius: 20px;
      padding: 40px;
      border: 1px solid #30363d;
      margin: 40px 0;
    }

    .annaba-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 25px;
      margin-top: 25px;
    }

    .annaba-item {
      position: relative;
      height: 240px;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 4px 15px rgba(0,0,0,0.5);
    }

    .annaba-item img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.5s ease;
    }

    .annaba-item:hover img {
      transform: scale(1.08);
    }

    .annaba-desc {
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      padding: 15px;
      background: linear-gradient(transparent, rgba(0,0,0,0.85));
      color: #fff;
    }

    .annaba-desc h4 {
      color: var(--gold);
      font-size: 1.1rem;
    }

    /* 5. COASTAL STRIP (HORIZONTAL SCROLL / GRID) */
    .coastal-container {
      display: flex;
      gap: 25px;
      overflow-x: auto;
      padding-bottom: 25px;
      scrollbar-width: thin;
      scrollbar-color: var(--gold) #21262d;
    }

    .coastal-container::-webkit-scrollbar {
      height: 8px;
    }
    .coastal-container::-webkit-scrollbar-thumb {
      background-color: var(--gold);
      border-radius: 4px;
    }

    .coastal-card {
      min-width: 300px;
      max-width: 300px;
      background: var(--card-bg);
      border-radius: 12px;
      overflow: hidden;
      border: 1px solid #30363d;
      flex-shrink: 0;
    }

    .coastal-card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
    }

    .coastal-info {
      padding: 15px;
    }

    .coastal-info h4 {
      font-size: 1.2rem;
      color: var(--gold);
      margin-bottom: 5px;
    }

    .coastal-info p {
      font-size: 0.85rem;
      color: var(--text-muted);
      line-height: 1.4;
    }

    footer {
      text-align: center;
      padding: 40px;
      background: #06090e;
      border-top: 1px solid #21262d;
      color: var(--text-muted);
    }

    @media (max-width: 768px) {
      .hero-title { font-size: 2.3rem; }
      .hero-subtitle { font-size: 1rem; }
      section { padding: 50px 5%; }
    }
  </style>
</head>
<body>

  <!-- 1. HERO SECTION -->
  <header class="hero">
    <h1 class="hero-title">Dz-Tourism Visit Algeria</h1>
    <p class="hero-subtitle">Discover the jewel of North Africa — from the golden dunes of the Sahara to timeless coastal treasures.</p>
    <a href="#hotels" class="btn-gold"><i class="fa-solid fa-compass"></i> Start Exploring</a>
  </header>

  <!-- 2. HOTELS SECTION -->
  <section id="hotels">
    <div class="section-header">
      <h2 class="section-title">Luxury & Authentic Hotels</h2>
      <p class="section-sub">Experience true Algerian hospitality in top-rated accommodations</p>
    </div>

    <div class="hotels-grid">
      <!-- Hotel 1 -->
      <div class="card">
        <div class="card-img-wrap">
          <img src="https://images.unsplash.com/photo-1566073771259-6a8506099945?auto=format&fit=crop&w=600&q=80" alt="Hotel El Aurassi">
          <span class="badge-price">From $120/night</span>
        </div>
        <div class="card-content">
          <h3>El Aurassi Palace</h3>
          <div class="card-location"><i class="fa-solid fa-location-dot"></i> Algiers (Wilaya 16)</div>
          <div class="rating">
            <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i> (4.9 / 5)
          </div>
          <a href="#" class="btn-book">Book Now</a>
        </div>
      </div>

      <!-- Hotel 2 -->
      <div class="card">
        <div class="card-img-wrap">
          <img src="https://images.unsplash.com/photo-1582719478250-c89cae4dc85b?auto=format&fit=crop&w=600&q=80" alt="Royal Hotel Oran">
          <span class="badge-price">From $95/night</span>
        </div>
        <div class="card-content">
          <h3>Royal Hotel Oran</h3>
          <div class="card-location"><i class="fa-solid fa-location-dot"></i> Oran (Wilaya 31)</div>
          <div class="rating">
            <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-regular fa-star"></i> (4.7 / 5)
          </div>
          <a href="#" class="btn-book">Book Now</a>
        </div>
      </div>

      <!-- Hotel 3 -->
      <div class="card">
        <div class="card-img-wrap">
          <img src="https://images.unsplash.com/photo-1571896349842-33c89424de2d?auto=format&fit=crop&w=600&q=80" alt="Sahara Oasis Lodge">
          <span class="badge-price">From $110/night</span>
        </div>
        <div class="card-content">
          <h3>Taghit Oasis Resort</h3>
          <div class="card-location"><i class="fa-solid fa-location-dot"></i> Béchar / Taghit</div>
          <div class="rating">
            <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i> (5.0 / 5)
          </div>
          <a href="#" class="btn-book">Book Now</a>
        </div>
      </div>
    </div>
  </section>

  <!-- 3. TRAVEL AGENCIES -->
  <section id="agencies" style="background:#0b0e14;">
    <div class="section-header">
      <h2 class="section-title">Certified Tourism Agencies</h2>
      <p class="section-sub">Guided Sahara expeditions, historic tours, and luxury car rentals</p>
    </div>

    <div class="agencies-grid">
      <div class="agency-card">
        <div class="agency-icon"><i class="fa-solid fa-car-side"></i></div>
        <h3>Sahara Wheels & Safari</h3>
        <p>4x4 desert expeditions across Djanet, Hoggar & Tassili n'Ajjer with certified guides.</p>
        <a href="#" class="btn-book">Contact Agency</a>
      </div>

      <div class="agency-card">
        <div class="agency-icon"><i class="fa-solid fa-map-location-dot"></i></div>
        <h3>Numidia Heritage Tours</h3>
        <p>Expert historic guidance exploring Roman ruins, Casbah of Algiers, and ancient monuments.</p>
        <a href="#" class="btn-book">View Packages</a>
      </div>

      <div class="agency-card">
        <div class="agency-icon"><i class="fa-solid fa-spa"></i></div>
        <h3>Royal Algerian Spa & Retreat</h3>
        <p>Thermal springs (Hammam Meskhoutine), relaxation, and massage wellness packages.</p>
        <a href="#" class="btn-book">Book Session</a>
      </div>
    </div>
  </section>

  <!-- 4. ANNABA SHOWCASE (THE PEARL OF EAST) -->
  <section id="annaba">
    <div class="annaba-showcase">
      <div class="section-header" style="margin-bottom: 20px;">
        <h2 class="section-title" style="color:#fbe29d;">Annaba (Bône) — The Ancient Hippo Regius</h2>
        <p class="section-sub">Ruins of Saint Augustine's basilica, turquoise Mediterranean bays, and lush green mountains</p>
      </div>

      <div class="annaba-grid">
        <div class="annaba-item">
          <img src="https://images.unsplash.com/photo-1544620347-c4fd4a3d5957?auto=format&fit=crop&w=600&q=80" alt="Roman Ruins Hippo Regius">
          <div class="annaba-desc">
            <h4>Hippo Regius Ruins</h4>
            <p>Ancient Roman forum, basilica & centuries-old mosaics</p>
          </div>
        </div>

        <div class="annaba-item">
          <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=600&q=80" alt="Seraïdi & Ain Achir Beach">
          <div class="annaba-desc">
            <h4>Seraïdi & Ain Achir Bay</h4>
            <p>Panoramic mountain views meeting the crystal turquoise sea</p>
          </div>
        </div>

        <div class="annaba-item">
          <img src="https://images.unsplash.com/photo-1519046904884-53103b34b206?auto=format&fit=crop&w=600&q=80" alt="Saint Augustin Basilica">
          <div class="annaba-desc">
            <h4>Saint Augustine Basilica</h4>
            <p>Monumental architectural masterpiece overlooking the coastline</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 5. COASTAL STRIP (EVERY COASTAL WILAYA) -->
  <section id="coast">
    <div class="section-header">
      <h2 class="section-title">The Algerian Coastal Strip</h2>
      <p class="section-sub">1,600+ km of Mediterranean beauty, historic forts, and natural wonder</p>
    </div>

    <div class="coastal-container">
      <!-- Tipaza -->
      <div class="coastal-card">
        <img src="https://images.unsplash.com/photo-1552832230-c0197dd311b5?auto=format&fit=crop&w=400&q=80" alt="Tipaza">
        <div class="coastal-info">
          <h4>Tipaza (Wilaya 42)</h4>
          <p>UNESCO World Heritage Roman ruins touching the turquoise waves and the Royal Mauritanian Tomb.</p>
        </div>
      </div>

      <!-- Algiers -->
      <div class="coastal-card">
        <img src="https://images.unsplash.com/photo-1513694203232-719a280e022f?auto=format&fit=crop&w=400&q=80" alt="Algiers Casbah">
        <div class="coastal-info">
          <h4>Algiers (Wilaya 16)</h4>
          <p>Algiers La Blanche, the historic UNESCO Casbah, and the iconic Monument of Martyrs.</p>
        </div>
      </div>

      <!-- Oran -->
      <div class="coastal-card">
        <img src="https://images.unsplash.com/photo-1548013146-72479768bada?auto=format&fit=crop&w=400&q=80" alt="Oran Santa Cruz">
        <div class="coastal-info">
          <h4>Oran (Wilaya 31)</h4>
          <p>The radiant El Bahia with the historic Fort of Santa Cruz overlooking the Mediterranean Gulf.</p>
        </div>
      </div>

      <!-- Bejaia -->
      <div class="coastal-card">
        <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=400&q=80" alt="Bejaia Cap Carbon">
        <div class="coastal-info">
          <h4>Béjaïa (Wilaya 06)</h4>
          <p>Dramatic towering cliffs of Cap Carbon, Yemma Gouraya peak, and Monkey Peak natural reserve.</p>
        </div>
      </div>

      <!-- Jijel -->
      <div class="coastal-card">
        <img src="https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?auto=format&fit=crop&w=400&q=80" alt="Jijel Caves">
        <div class="coastal-info">
          <h4>Jijel (Wilaya 18)</h4>
          <p>Emerald coast, mysterious caves (Grottes Merveilleuses), and virgin pine-tree shores.</p>
        </div>
      </div>

      <!-- Skikda -->
      <div class="coastal-card">
        <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=400&q=80" alt="Skikda Russicada">
        <div class="coastal-info">
          <h4>Skikda (Wilaya 21)</h4>
          <p>Ancient Russicada, neoclassical palace architecture, and stunning golden sandy beaches.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <p>© 2025 DZ-Tourism — Gateway to Algeria. Built with passion for Algeria's heritage.</p>
  </footer>

  <script>
    console.log("DZ-Tourism platform loaded successfully!");
  </script>
</body>
