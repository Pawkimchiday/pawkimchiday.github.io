<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>PAWKIMCHIDAY — Pet Treats & Goods</title>
  <meta name="description" content="PAWKIMCHIDAY — playful, pet‑safe treats and goods inspired by our Korean‑American home. Shop small, snack happy!" />
  <meta property="og:title" content="PAWKIMCHIDAY — Pet Treats & Goods" />
  <meta property="og:description" content="Playful, pet‑safe treats and goods inspired by our Korean‑American home." />
  <meta property="og:type" content="website" />
  <meta property="og:url" content="https://example.com" />
  <meta name="theme-color" content="#8B5E34" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Manrope:wght@300;400;600;800&family=Young+Serif&display=swap" rel="stylesheet">
  <style>
    :root{
      --brown:#8B5E34; --tan:#EAD7C3; --cream:#FFF9F3; --ink:#1F2937; --accent:#D9480F; --green:#0F766E;
      --radius:18px; --shadow:0 10px 25px rgba(0,0,0,.08);
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{margin:0;font-family:Manrope,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial,sans-serif;color:var(--ink);background:var(--cream)}
    a{color:var(--brown);text-decoration:none}
    img{max-width:100%;display:block}
    .container{width:min(1100px,92%);margin-inline:auto}
    /* Header */
    header{position:sticky;top:0;z-index:50;background:rgba(255,249,243,.8);backdrop-filter:saturate(180%) blur(10px);border-bottom:1px solid #f0e7db}
    .nav{display:flex;align-items:center;justify-content:space-between;padding:12px 0}
    .brand{display:flex;gap:10px;align-items:center}
    .brand-logo{width:40px;height:40px;border-radius:50%;background:conic-gradient(from 45deg at 50% 50%, var(--brown), var(--accent), var(--tan));box-shadow:var(--shadow)}
    .brand h1{font:800 20px/1 Young Serif, serif;margin:0;color:var(--brown)}
    nav ul{display:flex;gap:18px;list-style:none;margin:0;padding:0}
    nav a{padding:8px 12px;border-radius:999px}
    nav a:hover{background:var(--tan)}
    .menu-btn{display:none}
    @media (max-width:760px){
      nav ul{display:none;position:absolute;right:4%;top:64px;background:var(--cream);padding:14px;border-radius:var(--radius);box-shadow:var(--shadow);flex-direction:column}
      .menu-btn{display:inline-flex;align-items:center;gap:8px;padding:8px 12px;border:1px solid #e7d9c8;border-radius:999px;background:#fff}
      .menu-open nav ul{display:flex}
    }

    /* Hero */
    .hero{padding:72px 0 36px;background:linear-gradient(180deg, #fff, var(--cream));}
    .hero .wrap{display:grid;grid-template-columns:1.2fr 1fr;gap:40px;align-items:center}
    .badge{display:inline-flex;align-items:center;gap:8px;background:var(--tan);padding:6px 12px;border-radius:999px;font-weight:600;border:1px solid #e7d9c8}
    .title{font:800 44px/1.1 Young Serif, serif;margin:14px 0;color:var(--ink)}
    .subtitle{font-weight:400;color:#4b5563}
    .cta{display:flex;gap:12px;margin-top:22px}
    .btn{display:inline-flex;align-items:center;gap:8px;padding:12px 18px;border-radius:999px;border:2px solid var(--brown);font-weight:700}
    .btn.primary{background:var(--brown);color:#fff;border-color:var(--brown)}
    .btn.ghost:hover{background:var(--tan)}
    .hero-card{background:#fff;padding:16px;border-radius:var(--radius);box-shadow:var(--shadow);border:1px solid #f0e7db}
    .hero-card h3{margin:0 0 8px 0;font:800 18px/1 Young Serif, serif;color:var(--brown)}
    .hero-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-top:12px}
    .tag{font-size:12px;background:#FCEFE6;color:#7C2D12;padding:6px 10px;border-radius:999px;display:inline-block}
    @media (max-width:960px){.hero .wrap{grid-template-columns:1fr}}

    /* Sections */
    section{padding:56px 0}
    .section-title{font:800 28px/1 Young Serif, serif;color:var(--brown);margin:0 0 18px}
    .grid{display:grid;gap:18px}
    .grid.cols-3{grid-template-columns:repeat(3,1fr)}
    .grid.cols-2{grid-template-columns:repeat(2,1fr)}
    @media (max-width:900px){.grid.cols-3{grid-template-columns:1fr 1fr}}
    @media (max-width:640px){.grid.cols-3,.grid.cols-2{grid-template-columns:1fr}}

    .card{background:#fff;border:1px solid #f0e7db;border-radius:var(--radius);box-shadow:var(--shadow);padding:16px}
    .price{font-weight:800;color:var(--green)}

    /* Footer */
    footer{padding:36px 0;background:#fff;border-top:1px solid #f0e7db}
    .foot{display:flex;gap:24px;justify-content:space-between;align-items:center;flex-wrap:wrap}
    .social a{display:inline-flex;align-items:center;gap:8px;padding:8px 12px;border-radius:999px;border:1px solid #e7d9c8}
    .small{font-size:12px;color:#6b7280}
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">
        <div class="brand-logo" aria-hidden="true"></div>
        <h1>PAWKIMCHIDAY</h1>
      </div>
      <button class="menu-btn" aria-label="Toggle menu" onclick="document.body.classList.toggle('menu-open')">☰ Menu</button>
      <nav>
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#products">Products</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#pets">Our Pets</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <main id="home" class="hero">
    <div class="container wrap">
      <div>
        <span class="badge">🐾 Small batch • Vet‑friendly ingredients</span>
        <h2 class="title">Treats & goods made with love for pets in a Korean‑American home</h2>
        <p class="subtitle">No spicy flavors — just wholesome, pet‑safe recipes and playful designs that nod to our heritage.</p>
        <div class="cta">
          <a class="btn primary" href="#products">Shop Featured</a>
          <a class="btn ghost" href="#about">Learn More</a>
        </div>
      </div>
      <aside class="hero-card">
        <h3>Today’s Highlights</h3>
        <div class="hero-grid">
          <div class="card">
            <strong>100% grassfed organic jerky</strong>
            <p class="small">Single‑protein: 100% organic grassfed beef with no fillers.</p>
            <span class="tag">Grain‑free</span>
          </div>
          <div class="card">
            <strong>Chew bundle</strong>
            <p class="small">Pumpkin bites + ginger nibbles.</p>
            <span class="tag">Limited</span>
          </div>
        </div>
      </aside>
    </div>
  </main>

  <section id="products">
    <div class="container">
      <h2 class="section-title">Featured Products</h2>
      <div class="grid cols-3">
        <article class="card">
          <img src="https://images.unsplash.com/photo-1568640347023-a616a30bc3bd?q=80&w=1600&auto=format&fit=crop" alt="Chicken jerky for dogs">
          <h3>100% Grassfed Organic Beef Jerky</h3>
          <p>Lean, oven‑dried slices. No salt, no sugar, just protein.</p>
          <p class="price">$10.99</p>
          <a class="btn" href="#contact">Order</a>
        </article>
        <article class="card">
          <img src="https://images.unsplash.com/photo-1568641174277-4f70b10bd0f5?q=80&w=1600&auto=format&fit=crop" alt="Pumpkin dog treats">
          <h3>Organic Butternut Squash Bites</h3>
          <p>Soft treats with butternut squash slices. Great for sensitive tummies.</p>
          <p class="price">$5.99</p>
          <a class="btn" href="#contact">Order</a>
        </article>
        <article class="card">
          <img src="https://images.unsplash.com/photo-1612539722392-b496a7ce6fc0?q=80&w=1600&auto=format&fit=crop" alt="Rope toy with neutral colors">
          <h3>Dehydrated chicken neck</h3>
          <p>Homemade dehydrated chicken necks. Great dental chew alternatives.</p>
          <p class="price">$1.00 ea.</p>
          <a class="btn" href="#contact">Order</a>
        </article>
      </div>
    </div>
  </section>

  <section id="about" style="background:var(--tan)">
    <div class="container">
      <h2 class="section-title">Our Story</h2>
      <div class="grid cols-2">
        <div class="card" style="background:#fff">
          <p>We’re June + Michelle — Korean‑American pet parents. Our pets inspired us to create treats that we trust, and our pets can enjoy. No gochugaru here — just gentle, pet‑friendly ingredients and cozy aesthetics.</p>
          <ul>
            <li>Small‑batch, hand‑finished</li>
            <li>No artificial colors or preservatives</li>
            <li>Packaging that sparks a smile</li>
          </ul>
        </div>
        <div class="card" style="background:#fff">
          <h3 style="margin-top:0">Where to find us</h3>
          <p>Catch drops on Instagram and local pop‑ups. Nationwide shipping coming soon.</p>
          <p><strong>IG:</strong> <a href="https://instagram.com/pawkimchiday" target="_blank" rel="noopener">@pawkimchiday</a></p>
        </div>
      </div>
    </div>
  </section>

  <section id="pets">
    <div class="container">
      <h2 class="section-title">Meet Haku, Hanu & Bami</h2>
      <div class="grid cols-3">
        <figure class="card">
          <img src="https://images.unsplash.com/photo-1548199973-03cce0bbc87b?q=80&w=1600&auto=format&fit=crop" alt="Fluffy white dog">
          <figcaption class="small">Haku — floof ambassador & taste tester</figcaption>
        </figure>
        <figure class="card">
          <img src="https://images.unsplash.com/photo-1568572933382-74d440642117?q=80&w=1600&auto=format&fit=crop" alt="Tan medium dog">
          <figcaption class="small">Hanu — zoomie specialist</figcaption>
        </figure>
        <figure class="card">
          <img src="https://images.unsplash.com/photo-1518791841217-8f162f1e1131?q=80&w=1600&auto=format&fit=crop" alt="Calico cat relaxing">
          <figcaption class="small">Bami — quality control (strict)</figcaption>
        </figure>
      </div>
    </div>
  </section>

  <section id="faq" style="background:#fff">
    <div class="container">
      <h2 class="section-title">FAQ</h2>
      <div class="grid cols-2">
        <div class="card">
          <h3 style="margin-top:0">Are your treats spicy?</h3>
          <p>Never. We don’t use chili, garlic, onion, or anything unsafe for pets.</p>
        </div>
        <div class="card">
          <h3 style="margin-top:0">Do you ship?</h3>
          <p>Local pickup now; U.S. shipping coming soon. DM us on Instagram for custom orders.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="contact" style="background:var(--tan)">
    <div class="container">
      <h2 class="section-title">Get in Touch</h2>
      <div class="grid cols-2">
        <form class="card" style="background:#fff" onsubmit="alert('Thanks! This demo form uses mailto:—replace with Formspree or Netlify Forms when you publish.');">
          <label class="small" for="name">Name</label>
          <input id="name" name="name" required style="width:100%;padding:12px;border-radius:12px;border:1px solid #e5e7eb;margin:6px 0 12px">
          <label class="small" for="email">Email</label>
          <input id="email" name="email" type="email" required style="width:100%;padding:12px;border-radius:12px;border:1px solid #e5e7eb;margin:6px 0 12px">
          <label class="small" for="msg">Message</label>
          <textarea id="msg" name="message" rows="4" style="width:100%;padding:12px;border-radius:12px;border:1px solid #e5e7eb;margin:6px 0 12px"></textarea>
          <button class="btn primary" type="submit">Send</button>
        </form>
        <div class="card" style="background:#fff">
          <h3 style="margin-top:0">Email</h3>
          <p><a href="mailto:hello@pawkimchiday.example">hello@pawkimchiday.example</a></p>
          <h3>Instagram</h3>
          <p><a href="https://instagram.com/pawkimchiday" target="_blank" rel="noopener">@pawkimchiday</a></p>
          <h3>Pop‑ups</h3>
          <p class="small">We post dates on Stories. Come say hi!</p>
        </div>
      </div>
    </div>
  </section>

  <footer>
    <div class="container foot">
      <div class="brand" aria-label="Brand">
        <div class="brand-logo" aria-hidden="true"></div>
        <strong>PAWKIMCHIDAY</strong>
      </div>
      <div class="social">
        <a href="#contact">Email us</a>
        <a href="https://instagram.com/pawkimchiday" target="_blank" rel="noopener">Instagram</a>
      </div>
      <p class="small">© <span id="year"></span> PawkKimchiDay. All rights reserved.</p>
    </div>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
