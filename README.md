# ZEDMI
!DOCTYPE html>

<html lang="en">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">  
<title>Zedmi — Watches, Delivered</title>  
<style>  
  :root{  
    --bg:#f7f5f2; --surface:#ffffff; --text:#1a1a1a; --muted:#6b6b6b;  
    --accent:#b8893f; --accent-dark:#8a6529; --border:#e5e1da;  
    color-scheme: light dark;  
    box-sizing:border-box;  
    padding-top: env(safe-area-inset-top,0px);  
    padding-bottom: env(safe-area-inset-bottom,0px);  
  }  
  @media (prefers-color-scheme: dark){  
    :root:not([data-theme="light"]){  
      --bg:#121110; --surface:#1b1a18; --text:#f0ede6; --muted:#a8a29a;  
      --accent:#d9a85c; --accent-dark:#b8893f; --border:#2e2b26;  
    }  
  }  
  :root[data-theme="dark"]{  
    --bg:#121110; --surface:#1b1a18; --text:#f0ede6; --muted:#a8a29a;  
    --accent:#d9a85c; --accent-dark:#b8893f; --border:#2e2b26;  
  }  
  html{ scroll-padding-top: env(safe-area-inset-top,0px); }  
  *{ box-sizing:border-box; }  
  body{  
    margin:0; background:var(--bg); color:var(--text);  
    font-family:'Jost', -apple-system, 'Segoe UI', sans-serif;  
    -webkit-font-smoothing:antialiased;  
  }  
  body::before{  
    content:""; position:fixed; inset:0 0 auto; height:env(safe-area-inset-top,0px);  
    z-index:10; background:var(--bg);  
  }  
  header{  
    position:sticky; top:env(safe-area-inset-top,0px); z-index:5;  
    background:var(--bg); border-bottom:1px solid var(--border);  
    padding:18px 24px; display:flex; align-items:center; justify-content:space-between;  
  }  
  .logo{ font-size:1.4rem; font-weight:700; letter-spacing:2px; }  
  .logo span{ color:var(--accent); }  
  nav a{ color:var(--muted); text-decoration:none; margin-left:22px; font-size:.92rem; }  
  nav a:hover{ color:var(--accent); }  
  .hero{  
    text-align:center; padding:64px 20px 48px; max-width:720px; margin:0 auto;  
  }  
  .hero h1{ font-size:2.4rem; margin:0 0 14px; line-height:1.2; }  
  .hero h1 em{ font-style:normal; color:var(--accent); }  
  .hero p{ color:var(--muted); font-size:1.05rem; margin:0 0 26px; }  
  .cta{  
    display:inline-block; background:var(--accent); color:#1a1309; font-weight:600;  
    padding:13px 30px; border-radius:30px; text-decoration:none; font-size:.95rem;  
    transition:transform .15s ease;  
  }  
  .cta:hover{ transform:translateY(-2px); background:var(--accent-dark); }  
  .badges{  
    display:flex; justify-content:center; gap:28px; flex-wrap:wrap;  
    margin-top:36px; color:var(--muted); font-size:.82rem;  
  }  
  .badges div{ display:flex; align-items:center; gap:6px; }  
  section{ max-width:1080px; margin:0 auto; padding:40px 20px; }  
  h2{ font-size:1.5rem; text-align:center; margin-bottom:6px; }  
  .sub{ text-align:center; color:var(--muted); margin-bottom:34px; font-size:.95rem; }  
  .grid{  
    display:grid; grid-template-columns:repeat(auto-fit, minmax(220px,1fr)); gap:22px;  
  }  
  .card{  
    background:var(--surface); border:1px solid var(--border); border-radius:16px;  
    padding:22px; text-align:center; transition:transform .15s ease, box-shadow .15s ease;  
  }  
  .card:hover{ transform:translateY(-4px); box-shadow:0 10px 24px rgba(0,0,0,.08); }  
  .card svg{ width:100%; height:140px; margin-bottom:14px; }  
  .card h3{ margin:0 0 4px; font-size:1.05rem; }  
  .card .tag{ color:var(--muted); font-size:.8rem; margin-bottom:10px; }  
  .card .price{ color:var(--accent); font-weight:700; font-size:1.15rem; margin-bottom:14px; }  
  .buy{  
    display:inline-block; border:1px solid var(--accent); color:var(--accent);  
    padding:8px 20px; border-radius:24px; text-decoration:none; font-size:.85rem; font-weight:600;  
  }  
  .buy:hover{ background:var(--accent); color:#1a1309; }  
  .delivery{  
    background:var(--surface); border:1px solid var(--border); border-radius:20px;  
    padding:36px 28px; display:grid; grid-template-columns:repeat(auto-fit,minmax(200px,1fr)); gap:24px;  
  }  
  .d-item{ text-align:center; }  
  .d-item .ic{ font-size:1.8rem; margin-bottom:8px; }  
  .d-item h4{ margin:0 0 6px; font-size:1rem; }  
  .d-item p{ margin:0; color:var(--muted); font-size:.85rem; }  
  footer{  
    border-top:1px solid var(--border); text-align:center; padding:30px 20px;  
    color:var(--muted); font-size:.85rem;  
  }  
  footer .logo{ margin-bottom:8px; }  
  @media (max-width:560px){  
    .hero h1{ font-size:1.9rem; }  
    nav a{ margin-left:14px; font-size:.82rem; }  
  }  
</style>  
</head>  
<body>  <header>  
  <div class="logo">ZED<span>MI</span></div>  
  <nav>  
    <a href="#collection">Collection</a>  
    <a href="#delivery">Delivery</a>  
    <a href="#contact">Contact</a>  
  </nav>  
</header>  <div class="hero">  
  <h1>Timeless watches, <em>delivered to your door</em></h1>  
  <p>Zedmi brings you a curated collection of watches with fast, reliable delivery. Real products arriving soon — these are preview styles while our catalog is finalized.</p>  
  <a class="cta" href="#collection">Browse the collection</a>  
  <div class="badges">  
    <div>✓ coastal delivery</div>  
    <div>✓ Payment after delivery</div>  
    <div>✓ Authentic styles</div>  
  </div>  
</div>  <section id="collection">  
  <h2>Featured Watches</h2>  
  <p class="sub">Preview styles — your real product photos will replace these</p>  
  <div class="grid" id="product-grid"></div>  
</section>  <section id="delivery">  
  <h2>Delivery, done right</h2>  
  <p class="sub">Simple, tracked, and fast</p>  
  <div class="delivery">  
    <div class="d-item"><div class="ic"></div><h4>Nationwide shipping</h4><p>We deliver to every major town and city.</p></div>  
    <div class="d-item"><div class="ic"></div><h4>2–5 day delivery</h4><p>Most orders arrive within a working week.</p></div>  
    <div class="d-item"><div class="ic"></div><h4>Secure packaging</h4><p>Every watch is boxed and protected in transit.</p></div>  
    <div class="d-item"><div class="ic"></div><h4>Order tracking</h4><p>We keep you updated from checkout to doorstep.</p></div>  
  </div>  
</section>  <section id="contact">  
  <h2>Get in touch</h2>  
  <p class="sub">Questions about an order or want to place one? Reach out below.</p>  
  <div style="text-align:center; color:var(--muted); font-size:.95rem;">  
     orders@ iscovc2022@gmail.com &nbsp; | &nbsp;  WhatsApp us for quick replies:+254768115774  
  </div>  
</section>  <footer>  
  <div class="logo">ZED<span>MI</span></div>  
  Preview build — real product photos and checkout coming soon.  
</footer>  <script>  
// Simple SVG watch illustrations as placeholders (no external images)  
const styles = [  
  {name:"Classic Steel", tag:"Men's · Stainless", price:"KES 4,500", color:"#9aa0a6", band:"#c9cdd1"},  
  {name:"Rose Minimal", tag:"Women's · Leather", price:"KES 3,800", color:"#d9a85c", band:"#4a3a2a"},  
  {name:"Dive Pro", tag:"Men's · Sport", price:"KES 6,200", color:"#2b6e5c", band:"#1a1a1a"},  
  {name:"Gold Elegance", tag:"Unisex · Gold-tone", price:"KES 500", color:"#c9a24b", band:"#2a2a2a"},  
  {name:"Urban Black", tag:"Men's · Matte", price:"KES 4,200", color:"#2c2c2c", band:"#2c2c2c"},  
  {name:"Rose Chrono", tag:"Women's · Chronograph", price:"KES 400", color:"#b76e79", band:"#f0d9dc"}  
];  
  
function watchSVG(c){  
  return `<svg viewBox="0 0 200 160" xmlns="http://www.w3.org/2000/svg">  
    <rect x="86" y="8" width="28" height="20" rx="4" fill="${c.band}"/>  
    <rect x="86" y="132" width="28" height="20" rx="4" fill="${c.band}"/>  
    <circle cx="100" cy="80" r="46" fill="${c.color}" stroke="#00000022" stroke-width="2"/>  
    <circle cx="100" cy="80" r="38" fill="var(--surface)"/>  
    <line x1="100" y1="80" x2="100" y2="54" stroke="${c.color}" stroke-width="4" stroke-linecap="round"/>  
    <line x1="100" y1="80" x2="118" y2="88" stroke="${c.color}" stroke-width="3" stroke-linecap="round"/>  
    <circle cx="100" cy="80" r="3" fill="${c.color}"/>  
    <circle cx="100" cy="46" r="2" fill="${c.color}"/>  
    <circle cx="100" cy="114" r="2" fill="${c.color}"/>  
    <circle cx="66" cy="80" r="2" fill="${c.color}"/>  
    <circle cx="134" cy="80" r="2" fill="${c.color}"/>  
  </svg>`;  
}  
  
const grid = document.getElementById('product-grid');  
grid.innerHTML = styles.map(s => `  
  <div class="card">  
    ${watchSVG(s)}  
    <h3>${s.name}</h3>  
    <div class="tag">${s.tag}</div>  
    <div class="price">${s.price}</div>  
    <a class="buy" href="#contact">Order now</a>  
  </div>  
`).join('');  
</script>  </body>  
</html>  