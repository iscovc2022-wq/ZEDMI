<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Zedmi — Watches, Delivered</title>
<meta name="description" content="Zedmi brings you a curated collection of watches with fast, reliable delivery and payment after delivery.">
<meta name="description" content="Zedmi brings you a curated collection of watches with fast, reliable delivery and M-Pesa payment after delivery.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Jost:wght@400;600;700&display=swap" rel="stylesheet">
  <nav>
    <a href="#collection">Collection</a>
    <a href="#delivery">Delivery</a>
    <a href="#payment">Payment</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<div class="hero">
  <h1>Timeless watches, <em>delivered to your door</em></h1>
  <p>Zedmi brings you a curated collection of watches with fast, reliable delivery. Real products arriving soon — these are preview styles while our catalog is finalized.</p>
  <p>Karibuni nyote</p>
  <a class="cta" href="#collection">Browse the collection</a>
  <div class="badges">
    <div>Coastal delivery</div>
    <div>Payment after delivery</div>
    <div>Pay with M-Pesa after delivery</div>
    <div>Authentic styles</div>
  </div>
</div>
  </div>
</section>

<section id="payment">
  <h2>Payment</h2>
  <p class="sub">Pay with M-Pesa once your watch arrives</p>
  <div class="delivery">
    <div class="d-item"><h4>M-Pesa</h4><p>We accept payment through M-Pesa.</p></div>
    <div class="d-item"><h4>Pay after delivery</h4><p>Check your watch first, then pay. Nothing is due upfront.</p></div>
    <div class="d-item"><h4>Payment details on WhatsApp</h4><p>We send you the M-Pesa details when we confirm your order.</p></div>
  </div>
</section>

<section id="contact">
  <h2>Get in touch</h2>
  <p class="sub">Questions about an order or want to place one? Reach out below.</p>

<footer>
  <div class="logo">ZED<span>MI</span></div>
  Preview build — real product photos and checkout coming soon.
</footer>

<script>

const grid = document.getElementById('product-grid');
grid.innerHTML = styles.map(s => {
  const msg = encodeURIComponent(`Hi Zedmi, I'd like to order the ${s.name} (${s.price}).`);
  const msg = encodeURIComponent(`Hi Zedmi, I'd like to order the ${s.name} (${s.price}). I'll pay with M-Pesa on delivery.`);
  return `
  <div class="card">
    ${watchSVG(s)}  