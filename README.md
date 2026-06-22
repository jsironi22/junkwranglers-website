<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Junk Wranglers | Junk Removal Bozeman MT</title>
  <meta name="description" content="Fast, affordable junk removal in Bozeman, Belgrade, and Gallatin Valley. Furniture removal, appliance removal, garage cleanouts, and more. Call 406-970-3537.">

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Black+Han+Sans&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">

  <style>
    *, *::before, *::after {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    :root {
      --charcoal: #1a1a1a;
      --rust: #d4500a;
      --rust-dark: #a83d07;
      --cream: #f5f0e8;
      --mid-grey: #888;
      --light-grey: #e8e3da;
      --white: #ffffff;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      background: var(--cream);
      color: var(--charcoal);
      font-family: 'Inter', Arial, sans-serif;
      font-size: 16px;
      line-height: 1.6;
    }

    /* ─── NAV ─── */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 100;
      background: var(--charcoal);
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 32px;
      height: 60px;
    }

    .nav-logo {
      font-family: 'Black Han Sans', sans-serif;
      color: var(--white);
      font-size: 20px;
      letter-spacing: 0.04em;
      text-decoration: none;
    }

    .nav-logo span {
      color: var(--rust);
    }

    .nav-cta {
      background: var(--rust);
      color: var(--white);
      text-decoration: none;
      font-weight: 700;
      font-size: 14px;
      padding: 10px 20px;
      border-radius: 6px;
      letter-spacing: 0.04em;
      transition: background 0.2s;
    }

    .nav-cta:hover {
      background: var(--rust-dark);
    }

    /* ─── HERO ─── */
    .hero {
      min-height: 100vh;
      background: var(--charcoal);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 100px 24px 80px;
      position: relative;
      overflow: hidden;
    }

    /* Big diagonal texture lines */
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background: repeating-linear-gradient(
        -45deg,
        transparent,
        transparent 40px,
        rgba(255,255,255,0.018) 40px,
        rgba(255,255,255,0.018) 41px
      );
      pointer-events: none;
    }

    .hero-eyebrow {
      display: inline-block;
      background: var(--rust);
      color: var(--white);
      font-size: 12px;
      font-weight: 700;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      padding: 6px 16px;
      border-radius: 4px;
      margin-bottom: 28px;
    }

    .hero h1 {
      font-family: 'Black Han Sans', sans-serif;
      font-size: clamp(56px, 11vw, 110px);
      color: var(--white);
      line-height: 0.9;
      letter-spacing: -0.01em;
      margin-bottom: 8px;
    }

    .hero h1 .accent {
      color: var(--rust);
    }

    .hero-sub {
      font-family: 'Black Han Sans', sans-serif;
      font-size: clamp(20px, 4vw, 38px);
      color: rgba(255,255,255,0.55);
      letter-spacing: 0.06em;
      text-transform: uppercase;
      margin-bottom: 32px;
    }

    .hero-desc {
      max-width: 480px;
      color: rgba(255,255,255,0.65);
      font-size: 17px;
      margin-bottom: 44px;
      line-height: 1.7;
    }

    .hero-buttons {
      display: flex;
      gap: 14px;
      flex-wrap: wrap;
      justify-content: center;
    }

    .btn-call {
      background: var(--rust);
      color: var(--white);
      text-decoration: none;
      font-weight: 700;
      font-size: 17px;
      padding: 16px 36px;
      border-radius: 8px;
      letter-spacing: 0.02em;
      transition: background 0.2s, transform 0.15s;
      display: inline-flex;
      align-items: center;
      gap: 10px;
    }

    .btn-call:hover {
      background: var(--rust-dark);
      transform: translateY(-2px);
    }

    .btn-text {
      border: 2px solid rgba(255,255,255,0.25);
      color: var(--white);
      text-decoration: none;
      font-weight: 600;
      font-size: 17px;
      padding: 16px 36px;
      border-radius: 8px;
      transition: border-color 0.2s, transform 0.15s;
      display: inline-flex;
      align-items: center;
      gap: 10px;
    }

    .btn-text:hover {
      border-color: rgba(255,255,255,0.6);
      transform: translateY(-2px);
    }

    .hero-scroll {
      position: absolute;
      bottom: 32px;
      left: 50%;
      transform: translateX(-50%);
      color: rgba(255,255,255,0.3);
      font-size: 12px;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 8px;
    }

    .scroll-line {
      width: 1px;
      height: 40px;
      background: linear-gradient(to bottom, rgba(255,255,255,0.3), transparent);
    }

    /* ─── TRUST BAR ─── */
    .trust-bar {
      background: var(--rust);
      padding: 16px 24px;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 0;
    }

    .trust-item {
      color: var(--white);
      font-weight: 700;
      font-size: 14px;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      padding: 6px 28px;
      display: flex;
      align-items: center;
      gap: 8px;
      border-right: 1px solid rgba(255,255,255,0.3);
    }

    .trust-item:last-child {
      border-right: none;
    }

    /* ─── SERVICES ─── */
    .services {
      background: var(--cream);
      padding: 100px 24px;
    }

    .section-inner {
      max-width: 1040px;
      margin: 0 auto;
    }

    .section-label {
      font-size: 12px;
      font-weight: 700;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--rust);
      margin-bottom: 12px;
    }

    .section-title {
      font-family: 'Black Han Sans', sans-serif;
      font-size: clamp(36px, 5vw, 58px);
      color: var(--charcoal);
      line-height: 1;
      margin-bottom: 60px;
    }

    .services-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2px;
      border: 2px solid var(--charcoal);
    }

    .service-card {
      background: var(--white);
      padding: 36px 32px;
      border: 2px solid transparent;
      transition: background 0.2s;
      position: relative;
    }

    .service-card:hover {
      background: var(--charcoal);
    }

    .service-card:hover .service-name,
    .service-card:hover .service-desc {
      color: var(--white);
    }

    .service-card:hover .service-number {
      color: var(--rust);
    }

    .service-number {
      font-family: 'Black Han Sans', sans-serif;
      font-size: 13px;
      letter-spacing: 0.1em;
      color: var(--mid-grey);
      margin-bottom: 14px;
      transition: color 0.2s;
    }

    .service-icon {
      font-size: 28px;
      margin-bottom: 14px;
      display: block;
    }

    .service-name {
      font-family: 'Black Han Sans', sans-serif;
      font-size: 22px;
      color: var(--charcoal);
      margin-bottom: 10px;
      transition: color 0.2s;
    }

    .service-desc {
      color: #666;
      font-size: 15px;
      line-height: 1.6;
      transition: color 0.2s;
    }

    /* ─── HOW IT WORKS ─── */
    .how {
      background: var(--charcoal);
      padding: 100px 24px;
      color: var(--white);
    }

    .how .section-title {
      color: var(--white);
    }

    .steps {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 48px;
      margin-top: 0;
    }

    .step {
      position: relative;
    }

    .step-num {
      font-family: 'Black Han Sans', sans-serif;
      font-size: 64px;
      color: var(--rust);
      line-height: 1;
      margin-bottom: 18px;
    }

    .step-title {
      font-family: 'Black Han Sans', sans-serif;
      font-size: 22px;
      color: var(--white);
      margin-bottom: 10px;
    }

    .step-desc {
      color: rgba(255,255,255,0.55);
      font-size: 15px;
      line-height: 1.7;
    }

    /* ─── AREA ─── */
    .area {
      background: var(--light-grey);
      padding: 100px 24px;
    }

    .area-inner {
      max-width: 1040px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 80px;
      align-items: start;
    }

    .area-towns {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 32px;
    }

    .town-tag {
      background: var(--charcoal);
      color: var(--white);
      padding: 8px 18px;
      border-radius: 40px;
      font-size: 14px;
      font-weight: 600;
    }

    .area-note {
      color: #666;
      font-size: 15px;
      margin-top: 20px;
      line-height: 1.7;
    }

    .area-highlight {
      background: var(--charcoal);
      border-radius: 16px;
      padding: 48px 40px;
      color: var(--white);
    }

    .area-highlight h3 {
      font-family: 'Black Han Sans', sans-serif;
      font-size: 28px;
      color: var(--white);
      margin-bottom: 20px;
      line-height: 1.2;
    }

    .area-highlight p {
      color: rgba(255,255,255,0.6);
      font-size: 15px;
      line-height: 1.7;
      margin-bottom: 28px;
    }

    .area-phone {
      display: flex;
      align-items: center;
      gap: 12px;
      color: var(--rust);
      font-family: 'Black Han Sans', sans-serif;
      font-size: 28px;
      text-decoration: none;
      letter-spacing: 0.02em;
      transition: opacity 0.2s;
    }

    .area-phone:hover {
      opacity: 0.8;
    }

    /* ─── CTA ─── */
    .final-cta {
      background: var(--rust);
      padding: 100px 24px;
      text-align: center;
    }

    .final-cta h2 {
      font-family: 'Black Han Sans', sans-serif;
      font-size: clamp(40px, 7vw, 72px);
      color: var(--white);
      line-height: 1;
      margin-bottom: 20px;
    }

    .final-cta p {
      color: rgba(255,255,255,0.75);
      font-size: 18px;
      margin-bottom: 40px;
    }

    .btn-white {
      background: var(--white);
      color: var(--rust);
      text-decoration: none;
      font-weight: 800;
      font-size: 18px;
      padding: 18px 44px;
      border-radius: 8px;
      display: inline-block;
      letter-spacing: 0.02em;
      transition: transform 0.15s, box-shadow 0.15s;
      box-shadow: 0 4px 20px rgba(0,0,0,0.2);
    }

    .btn-white:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 28px rgba(0,0,0,0.25);
    }

    /* ─── FOOTER ─── */
    footer {
      background: var(--charcoal);
      padding: 40px 24px;
      text-align: center;
    }

    .footer-logo {
      font-family: 'Black Han Sans', sans-serif;
      font-size: 24px;
      color: var(--white);
      letter-spacing: 0.04em;
      margin-bottom: 10px;
    }

    .footer-logo span {
      color: var(--rust);
    }

    .footer-tagline {
      color: rgba(255,255,255,0.35);
      font-size: 14px;
      margin-bottom: 24px;
      letter-spacing: 0.03em;
    }

    .footer-links {
      display: flex;
      justify-content: center;
      gap: 24px;
      flex-wrap: wrap;
    }

    .footer-links a {
      color: rgba(255,255,255,0.45);
      text-decoration: none;
      font-size: 14px;
      transition: color 0.2s;
    }

    .footer-links a:hover {
      color: var(--rust);
    }

    /* ─── MOBILE ─── */
    @media (max-width: 700px) {
      nav {
        padding: 0 20px;
      }

      .trust-item {
        padding: 6px 16px;
        font-size: 12px;
        border-right: none;
        border-bottom: 1px solid rgba(255,255,255,0.2);
      }

      .trust-item:last-child {
        border-bottom: none;
      }

      .trust-bar {
        flex-direction: column;
        align-items: center;
        gap: 0;
      }

      .services-grid {
        grid-template-columns: 1fr;
      }

      .area-inner {
        grid-template-columns: 1fr;
        gap: 40px;
      }

      .steps {
        gap: 36px;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      * {
        transition: none !important;
      }
    }
  </style>
</head>

<body>

  <!-- NAV -->
  <nav>
    <a class="nav-logo" href="#">JUNK <span>WRANGLERS</span></a>
    <a class="nav-cta" href="tel:406-970-3537">406-970-3537</a>
  </nav>

  <!-- HERO -->
  <section class="hero">
    <div class="hero-eyebrow">Bozeman &amp; Gallatin Valley</div>

    <h1>JUNK<br><span class="accent">WRANGLERS</span></h1>
    <p class="hero-sub">We haul it. You reclaim it.</p>

    <p class="hero-desc">
      Same-day junk removal across the Gallatin Valley. Furniture, appliances, garage cleanouts, yard waste — if you need it gone, we're on our way.
    </p>

    <div class="hero-buttons">
      <a class="btn-call" href="tel:406-970-3537">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07A19.5 19.5 0 013.07 11a19.79 19.79 0 01-3.07-8.67A2 2 0 012 .18h3a2 2 0 012 1.72 12.84 12.84 0 00.7 2.81 2 2 0 01-.45 2.11L6.09 7.91a16 16 0 006 6l1.27-1.27a2 2 0 012.11-.45 12.84 12.84 0 002.81.7A2 2 0 0122 14h0z"></path></svg>
        Call Now
      </a>
      <a class="btn-text" href="sms:406-970-3537">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 01-2 2H7l-4 4V5a2 2 0 012-2h14a2 2 0 012 2z"></path></svg>
        Text a Photo
      </a>
    </div>

    <div class="hero-scroll">
      <div class="scroll-line"></div>
      Scroll
    </div>
  </section>

  <!-- TRUST BAR -->
  <div class="trust-bar">
    <div class="trust-item">✔ Same-Day Service</div>
    <div class="trust-item">✔ Honest Pricing</div>
    <div class="trust-item">✔ Locally Owned</div>
    <div class="trust-item">✔ No Hidden Fees</div>
  </div>

  <!-- SERVICES -->
  <section class="services">
    <div class="section-inner">
      <p class="section-label">What We Haul</p>
      <h2 class="section-title">We Wrangle<br>All of It</h2>

      <div class="services-grid">
        <div class="service-card">
          <div class="service-number">01</div>
          <span class="service-icon">🛋️</span>
          <h3 class="service-name">Furniture</h3>
          <p class="service-desc">Couches, beds, dressers, tables, recliners — bulky items are our specialty. No job too big.</p>
        </div>
        <div class="service-card">
          <div class="service-number">02</div>
          <span class="service-icon">🧺</span>
          <h3 class="service-name">Appliances</h3>
          <p class="service-desc">Fridges, washers, dryers, stoves, dishwashers. We handle the heavy lifting so you don't have to.</p>
        </div>
        <div class="service-card">
          <div class="service-number">03</div>
          <span class="service-icon">🏚️</span>
          <h3 class="service-name">Garage Cleanouts</h3>
          <p class="service-desc">Years of clutter, cleared out fast. We haul it all and leave your garage ready to actually use.</p>
        </div>
        <div class="service-card">
          <div class="service-number">04</div>
          <span class="service-icon">🌿</span>
          <h3 class="service-name">Yard Waste</h3>
          <p class="service-desc">Branches, brush, old fencing, landscaping debris — your yard, cleared and clean.</p>
        </div>
        <div class="service-card">
          <div class="service-number">05</div>
          <span class="service-icon">🏠</span>
          <h3 class="service-name">Estate Cleanouts</h3>
          <p class="service-desc">Respectful, thorough cleanouts for full properties. We treat every home with care.</p>
        </div>
        <div class="service-card">
          <div class="service-number">06</div>
          <span class="service-icon">🧱</span>
          <h3 class="service-name">Construction Debris</h3>
          <p class="service-desc">Renovation scraps, drywall, lumber, roofing materials. We clear the site so you can keep working.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- HOW IT WORKS -->
  <section class="how">
    <div class="section-inner">
      <p class="section-label">How It Works</p>
      <h2 class="section-title">Done in<br>Three Steps</h2>

      <div class="steps">
        <div class="step">
          <div class="step-num">1</div>
          <h3 class="step-title">Call or Text a Photo</h3>
          <p class="step-desc">Snap a photo of what you need gone and text it to us at 406-970-3537, or just give us a call. We'll get back to you fast with a fair, upfront price.</p>
        </div>
        <div class="step">
          <div class="step-num">2</div>
          <h3 class="step-title">We Show Up</h3>
          <p class="step-desc">Often same-day. Our crew arrives on time and gets straight to work. You don't lift a finger — we handle all the heavy hauling.</p>
        </div>
        <div class="step">
          <div class="step-num">3</div>
          <h3 class="step-title">You Reclaim Your Space</h3>
          <p class="step-desc">We load it, we haul it, we're gone. No mess left behind. Just clean, open space where that junk used to be.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- SERVICE AREA -->
  <section class="area">
    <div class="area-inner">
      <div>
        <p class="section-label">Service Area</p>
        <h2 class="section-title">Proudly Serving<br>Gallatin Valley</h2>
        <div class="area-towns">
          <span class="town-tag">Bozeman</span>
          <span class="town-tag">Belgrade</span>
          <span class="town-tag">Livingston</span>
          <span class="town-tag">Four Corners</span>
          <span class="town-tag">Manhattan</span>
          <span class="town-tag">Gallatin Gateway</span>
        </div>
        <p class="area-note">Not sure if we cover your area? Just call or text — we'll let you know. We work hard to say yes whenever we can.</p>
      </div>

      <div class="area-highlight">
        <h3>Ready to get that junk out of your life?</h3>
        <p>Call or text us a photo for a fast, no-obligation quote. We price honestly and show up when we say we will.</p>
        <a class="area-phone" href="tel:406-970-3537">
          <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07A19.5 19.5 0 013.07 11a19.79 19.79 0 01-3.07-8.67A2 2 0 012 .18h3a2 2 0 012 1.72 12.84 12.84 0 00.7 2.81 2 2 0 01-.45 2.11L6.09 7.91a16 16 0 006 6l1.27-1.27a2 2 0 012.11-.45 12.84 12.84 0 002.81.7A2 2 0 0122 14h0z"></path></svg>
          406-970-3537
        </a>
      </div>
    </div>
  </section>

  <!-- FINAL CTA -->
  <section class="final-cta">
    <h2>NEED IT<br>GONE TODAY?</h2>
    <p>Same-day service available across the Gallatin Valley. Call now — we'll make it happen.</p>
    <a class="btn-white" href="tel:406-970-3537">Call 406-970-3537</a>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="footer-logo">JUNK <span>WRANGLERS</span></div>
    <p class="footer-tagline">We wrangle the junk. You reclaim your space. — Bozeman, Montana</p>
    <div class="footer-links">
      <a href="tel:406-970-3537">406-970-3537</a>
      <a href="sms:406-970-3537">Text a Photo</a>
    </div>
  </footer>

</body>
</html>
