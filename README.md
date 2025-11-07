# lmds.clothing
Street wear clothing brand
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Le monde de Starr — Drop Dec 18</title>
  <meta name="description" content="Le monde de Starr — street luxe streetwear drop. Hoodie drop Dec 18. Join SMS list for early access." />
  <!-- Open Graph -->
  <meta property="og:title" content="Le monde de Starr — Drop Dec 18" />
  <meta property="og:description" content="Street luxe hoodie drop. Join SMS for early access & exclusive drops." />
  <meta property="og:image" content="assets/og-image.jpg" />
  <meta property="og:type" content="website" />
  <link rel="icon" href="assets/favicon.png" />
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="site-header">
    <div class="container">
      <a class="brand" href="#">Le monde de Starr</a>
      <nav class="nav">
        <a href="#drop">Drop</a>
        <a href="#sign-up">SMS</a>
        <a href="#about">About</a>
      </nav>
    </div>
  </header>

  <main>
    <!-- Hero -->
    <section class="hero" id="drop" aria-labelledby="hero-title">
      <div class="container hero-grid">
        <div class="hero-left">
          <h1 id="hero-title">LE MONDE DE STARR</h1>
          <p class="tagline">Street luxe. Raw. Limited.</p>
          <p class="lead">Hoodie drop — <strong>December 18</strong>. Limited run. Early access to SMS subscribers.</p>

          <div class="countdown" aria-live="polite">
            <div class="countdown-item"><span id="days">00</span><small>days</small></div>
            <div class="countdown-item"><span id="hours">00</span><small>hours</small></div>
            <div class="countdown-item"><span id="minutes">00</span><small>minutes</small></div>
            <div class="countdown-item"><span id="seconds">00</span><small>seconds</small></div>
          </div>

          <div class="cta-row">
            <a class="btn primary" href="#sign-up">Join SMS List</a>
            <a class="btn ghost" href="#about">Learn more</a>
          </div>

          <p class="small-note">Follow @lemonde_de_starr for behind-the-scenes + daily drops.</p>
        </div>

        <div class="hero-right">
          <!-- Placeholder product image -->
          <img src="assets/hoodie-mockup.jpg" alt="Hoodie mockup — Le monde de Starr" />
        </div>
      </div>
    </section>

    <!-- Sign up -->
    <section class="signup" id="sign-up" aria-labelledby="signup-title">
      <div class="container">
        <h2 id="signup-title">Get early access — SMS signup</h2>
        <p>Enter your phone number. We'll text you early access + exclusive codes.</p>

        <form id="sms-form" class="form" autocomplete="on">
          <label for="phone">Phone number</label>
          <input id="phone" name="phone" type="tel" placeholder="+1 555 555 5555" required pattern="^\+?[0-9\s\-()]{7,}$" />
          <label for="consent" class="consent">
            <input id="consent" name="consent" type="checkbox" required />
            I agree to receive SMS from Le monde de Starr. Message/data rates may apply.
          </label>

          <div class="form-actions">
            <button class="btn primary" type="submit">Join the list</button>
            <div id="form-status" role="status" aria-live="polite"></div>
          </div>
        </form>

        <p class="small-note">We respect your privacy. We won't spam—just exclusive drops & restock alerts.</p>
      </div>
    </section>

    <!-- About -->
    <section class="about" id="about" aria-labelledby="about-title">
      <div class="container">
        <h2 id="about-title">About Le monde de Starr</h2>
        <p>Le monde de Starr blends raw streetwear energy with luxe sensibility. Each piece is limited — designed for the ones who stand out.</p>

        <div class="features">
          <div class="feature">
            <h3>Limited runs</h3>
            <p>Small batch production keeps pieces rare and exclusive.</p>
          </div>
          <div class="feature">
            <h3>Quality & feel</h3>
            <p>Premium fabrics, heavy weight hoodies, and unique washes.</p>
          </div>
          <div class="feature">
            <h3>Community</h3>
            <p>Early access, VIP restock alerts, and collabs for SMS subscribers.</p>
          </div>
        </div>

        <footer class="site-footer">
          <div>© <span id="year"></span> Le monde de Starr</div>
          <div class="socials">
            <a href="https://instagram.com/lemonde_de_starr" target="_blank" rel="noopener">Instagram</a>
            <a href="https://twitter.com/lemonde_de_starr" target="_blank" rel="noopener">X</a>
          </div>
        </footer>
      </div>
    </section>
  </main>

  <script src="script.js"></script>
</body>
</html>
/* styles.css - simple, modern, responsive */
:root{
  --bg:#0b0b0b;
  --card:#0f0f0f;
  --muted:#bdbdbd;
  --accent:#ffffff;
  --accent-2:#e6e6e6;
  --gap:18px;
  --max-width:1100px;
  font-family: "Inter", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
}

*{box-sizing:border-box}
html,body{height:100%}
body{
  margin:0;
  background:linear-gradient(180deg,#050505,var(--bg));
  color:var(--accent-2);
  -webkit-font-smoothing:antialiased;
  -moz-osx-font-smoothing:grayscale;
  line-height:1.45;
}

.container{
  width:95%;
  max-width:var(--max-width);
  margin:0 auto;
}

.site-header{
  padding:18px 0;
  position:sticky;
  top:0;
  z-index:50;
  backdrop-filter: blur(6px);
  background:rgba(0,0,0,0.25);
}

.brand{
  color:var(--accent);
  font-weight:700;
  text-decoration:none;
  letter-spacing:0.08em;
}
.nav{float:right}
.nav a{color:var(--muted); margin-left:16px; text-decoration:none; font-size:0.95rem}

.hero{
  padding:48px 0;
  display:block;
}
.hero-grid{
  display:grid;
  grid-template-columns:1fr 420px;
  gap:36px;
  align-items:center;
}
.hero-left h1{
  font-size:2.4rem;
  margin:0 0 6px 0;
  letter-spacing:0.12em;
}
.tagline{color:var(--muted); margin:6px 0 12px 0; font-weight:600}
.lead{margin-bottom:18px; color:var(--accent-2)}

.hero-right img{
  width:100%;
  border-radius:8px;
  object-fit:cover;
  box-shadow:0 20px 40px rgba(0,0,0,0.6);
}

/* countdown */
.countdown{display:flex; gap:12px; margin:12px 0 18px 0}
.countdown-item{
  background:var(--card);
  padding:12px 18px;
  border-radius:10px;
  text-align:center;
  min-width:78px;
}
.countdown-item span{display:block; font-size:1.4rem; font-weight:700}
.countdown-item small{display:block; color:var(--muted); font-size:0.78rem}

/* buttons */
.btn{
  display:inline-block;
  padding:12px 18px;
  border-radius:8px;
  text-decoration:none;
  cursor:pointer;
  border:1px solid rgba(255,255,255,0.06);
  font-weight:700;
}
.btn.primary{background:var(--accent); color:#000}
.btn.ghost{background:transparent; color:var(--accent-2); border:1px solid rgba(255,255,255,0.06); margin-left:8px}

.cta-row{margin-top:12px}

/* signup section */
.signup{padding:40px 0; background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent)}
.form{max-width:520px}
.form label{display:block; font-size:0.9rem; margin-bottom:6px}
.form input[type="tel"]{
  width:100%; padding:12px; border-radius:8px; border:1px solid rgba(255,255,255,0.06); background:transparent; color:var(--accent-2)
}
.form .consent{display:flex; gap:10px; align-items:center; margin:12px 0; font-size:0.9rem; color:var(--muted)}
.form-actions{display:flex; gap:12px; align-items:center}
#form-status{color:var(--muted); font-size:0.9rem}

/* features */
.about{padding:36px 0}
.features{display:grid; grid-template-columns:repeat(3,1fr); gap:18px; margin-top:18px}
.feature{background:var(--card); padding:18px; border-radius:10px}

/* footer */
.site-footer{display:flex; justify-content:space-between; margin-top:26px; color:var(--muted); font-size:0.9rem}
.socials a{color:var(--muted); margin-left:12px; text-decoration:none}

/* responsive */
@media (max-width:980px){
  .hero-grid{grid-template-columns:1fr; text-align:center}
  .hero-right{order:-1}
  .nav{float:none; margin-top:8px}
  .site-header .container{display:flex; align-items:center; justify-content:space-between}
}
@media (max-width:640px){
  .features{grid-template-columns:1fr}
  .countdown-item{min-width:62px}
}
// script.js
document.addEventListener('DOMContentLoaded', () => {
  // Set current year
  document.getElementById('year').textContent = new Date().getFullYear();

  // Countdown target: December 18 of current year (if passed, target next year)
  const now = new Date();
  let targetYear = now.getFullYear();
  const dropDate = new Date(`${targetYear}-12-18T12:00:00`); // noon local time
  if (dropDate < now) dropDate.setFullYear(targetYear + 1);

  // Countdown update
  function updateCountdown() {
    const t = dropDate - new Date();
    if (t <= 0) {
      document.querySelector('.countdown').innerHTML = '<strong>Drop is live — shop now!</strong>';
      return;
    }
    const secs = Math.floor(t / 1000);
    const days = Math.floor(secs / 86400);
    const hours = Math.floor((secs % 86400) / 3600);
    const minutes = Math.floor((secs % 3600) / 60);
    const seconds = secs % 60;

    document.getElementById('days').textContent = String(days).padStart(2,'0');
    document.getElementById('hours').textContent = String(hours).padStart(2,'0');
    document.getElementById('minutes').textContent = String(minutes).padStart(2,'0');
    document.getElementById('seconds').textContent = String(seconds).padStart(2,'0');
  }
  updateCountdown();
  setInterval(updateCountdown, 1000);

  // SMS form submission
  const form = document.getElementById('sms-form');
  const status = document.getElementById('form-status');
  form.addEventListener('submit', async (e) => {
    e.preventDefault();
    status.textContent = 'Sending...';

    const phone = document.getElementById('phone').value;
    const consent = document.getElementById('consent').checked;
    if (!consent) {
      status.textContent = 'Please agree to receive SMS.';
      return;
    }

    try {
      const res = await fetch('/.netlify/functions/sms-signup', {
        method: 'POST',
        headers: {'Content-Type':'application/json'},
        body: JSON.stringify({ phone })
      });
      const data = await res.json();
      if (res.ok) {
        status.textContent = 'Thanks! You’re on the list — expect a text soon.';
        form.reset();
      } else {
        status.textContent = data.error || 'Something went wrong. Try again later.';
      }
    } catch (err) {
      console.error(err);
      status.textContent = 'Network error. Try again later.';
    }
  });
});
// sms-signup.js (Netlify Function)
const fetch = require('node-fetch'); // Netlify provides fetch in newer runtimes; otherwise add node-fetch
const twilio = require('twilio');

exports.handler = async (event, context) => {
  if (event.httpMethod !== 'POST') return { statusCode: 405, body: 'Method Not Allowed' };
  try {
    const body = JSON.parse(event.body);
    const phone = body.phone;
    if (!phone) return { statusCode: 400, body: JSON.stringify({ error: 'Missing phone' }) };

    const { TWILIO_ACCOUNT_SID, TWILIO_AUTH_TOKEN, TWILIO_FROM_NUMBER, ADMIN_NUMBER } = process.env;
    if (!TWILIO_ACCOUNT_SID || !TWILIO_AUTH_TOKEN || !TWILIO_FROM_NUMBER) {
      return { statusCode: 500, body: JSON.stringify({ error: 'Twilio not configured' }) };
    }

    const client = twilio(TWILIO_ACCOUNT_SID, TWILIO_AUTH_TOKEN);

    // Send a confirmation text to the user (optional)
    await client.messages.create({
      body: 'Thanks for joining Le monde de Starr — you’ll get early access to the Dec 18 drop. Reply STOP to unsubscribe.',
      from: TWILIO_FROM_NUMBER,
      to: phone
    });

    // Notify admin/you about new signup (optional)
    if (ADMIN_NUMBER) {
      await client.messages.create({
        body: `New signup: ${phone}`,
        from: TWILIO_FROM_NUMBER,
        to: ADMIN_NUMBER
      });
    }

    return { statusCode: 200, body: JSON.stringify({ success: true }) };
  } catch (err) {
    console.error(err);
    return { statusCode: 500, body: JSON.stringify({ error: 'Server error' }) };
  }
};
