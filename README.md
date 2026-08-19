<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="Gold (GLD) — A new digital asset launching on BNB Smart Chain. Presale coming soon." />
  <title>Gold (GLD) — Coming Soon</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    :root {
      --gold: #d4af37;
      --gold-light: #f5d76e;
      --gold-dark: #9c7c18;
      --bg: #070707;
      --card: rgba(255, 255, 255, 0.055);
      --border: rgba(212, 175, 55, 0.2);
      --text: #f5f5f5;
      --muted: #a7a7a7;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Inter, -apple-system, BlinkMacSystemFont, "Segoe UI",
        Roboto, Helvetica, Arial, sans-serif;
      background:
        radial-gradient(circle at 50% -10%, rgba(212, 175, 55, 0.16), transparent 35%),
        radial-gradient(circle at 10% 80%, rgba(212, 175, 55, 0.06), transparent 30%),
        var(--bg);
      color: var(--text);
      min-height: 100vh;
      overflow-x: hidden;
    }

    /* Background particles */
    .particles {
      position: fixed;
      inset: 0;
      pointer-events: none;
      overflow: hidden;
      z-index: 0;
    }

    .particle {
      position: absolute;
      width: 3px;
      height: 3px;
      background: var(--gold);
      border-radius: 50%;
      opacity: 0.35;
      animation: float 8s infinite ease-in-out;
    }

    .particle:nth-child(1) { left: 8%; top: 20%; animation-delay: 0s; }
    .particle:nth-child(2) { left: 18%; top: 70%; animation-delay: 2s; }
    .particle:nth-child(3) { left: 32%; top: 35%; animation-delay: 4s; }
    .particle:nth-child(4) { left: 52%; top: 75%; animation-delay: 1s; }
    .particle:nth-child(5) { left: 68%; top: 25%; animation-delay: 3s; }
    .particle:nth-child(6) { left: 82%; top: 65%; animation-delay: 5s; }
    .particle:nth-child(7) { left: 92%; top: 18%; animation-delay: 2.5s; }
    .particle:nth-child(8) { left: 45%; top: 12%; animation-delay: 1.5s; }

    @keyframes float {
      0%, 100% {
        transform: translateY(0);
        opacity: 0.2;
      }
      50% {
        transform: translateY(-30px);
        opacity: 0.7;
      }
    }

    .container {
      width: min(1120px, 92%);
      margin: auto;
      position: relative;
      z-index: 1;
    }

    /* Navigation */
    nav {
      height: 80px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 12px;
      font-weight: 800;
      font-size: 22px;
      letter-spacing: 1px;
    }

    .logo-icon {
      width: 38px;
      height: 38px;
      border-radius: 50%;
      display: grid;
      place-items: center;
      background: linear-gradient(145deg, #f5d76e, #9c7c18);
      color: #111;
      font-weight: 900;
      box-shadow: 0 0 25px rgba(212, 175, 55, 0.25);
    }

    .network {
      border: 1px solid var(--border);
      background: rgba(212, 175, 55, 0.07);
      padding: 9px 14px;
      border-radius: 999px;
      font-size: 13px;
      color: var(--gold-light);
    }

    /* Hero */
    .hero {
      min-height: calc(100vh - 80px);
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 70px 0 90px;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 8px 14px;
      border-radius: 999px;
      border: 1px solid var(--border);
      background: rgba(212, 175, 55, 0.06);
      color: var(--gold-light);
      font-size: 13px;
      font-weight: 600;
      margin-bottom: 25px;
    }

    .badge-dot {
      width: 7px;
      height: 7px;
      background: var(--gold);
      border-radius: 50%;
      box-shadow: 0 0 10px var(--gold);
    }

    h1 {
      font-size: clamp(58px, 10vw, 120px);
      line-height: 0.95;
      letter-spacing: -5px;
      font-weight: 900;
      background: linear-gradient(
        135deg,
        #fff 15%,
        var(--gold-light) 45%,
        var(--gold-dark) 90%
      );
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      margin-bottom: 24px;
    }

    .subtitle {
      max-width: 680px;
      margin: auto;
      color: var(--muted);
      font-size: clamp(17px, 2vw, 21px);
      line-height: 1.7;
    }

    .highlight {
      color: var(--gold-light);
    }

    /* Countdown */
    .countdown-title {
      margin-top: 55px;
      margin-bottom: 18px;
      font-size: 13px;
      text-transform: uppercase;
      letter-spacing: 3px;
      color: #777;
    }

    .countdown {
      display: flex;
      justify-content: center;
      gap: 12px;
      flex-wrap: wrap;
    }

    .time-box {
      width: 105px;
      padding: 19px 10px;
      border: 1px solid var(--border);
      border-radius: 16px;
      background: var(--card);
      backdrop-filter: blur(12px);
    }

    .time-number {
      display: block;
      font-size: 32px;
      font-weight: 800;
      color: var(--gold-light);
    }

    .time-label {
      font-size: 10px;
      text-transform: uppercase;
      letter-spacing: 2px;
      color: #777;
      margin-top: 5px;
    }

    /* CTA */
    .buttons {
      display: flex;
      justify-content: center;
      gap: 12px;
      flex-wrap: wrap;
      margin-top: 38px;
    }

    .btn {
      border: none;
      text-decoration: none;
      padding: 14px 24px;
      border-radius: 12px;
      font-weight: 700;
      font-size: 14px;
      transition: 0.25s ease;
      cursor: pointer;
    }

    .btn-primary {
      background: linear-gradient(135deg, #f5d76e, #b18a1c);
      color: #111;
      box-shadow: 0 10px 30px rgba(212, 175, 55, 0.18);
    }

    .btn-primary:hover {
      transform: translateY(-2px);
      box-shadow: 0 14px 35px rgba(212, 175, 55, 0.3);
    }

    .btn-secondary {
      border: 1px solid var(--border);
      background: rgba(255,255,255,0.03);
      color: #ddd;
    }

    .btn-secondary:hover {
      border-color: rgba(212, 175, 55, 0.5);
      color: var(--gold-light);
    }

    /* Stats */
    .stats {
      width: min(850px, 100%);
      margin: 70px auto 0;
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 1px;
      background: var(--border);
      border: 1px solid var(--border);
      border-radius: 18px;
      overflow: hidden;
    }

    .stat {
      background: rgba(10,10,10,0.92);
      padding: 28px 15px;
    }

    .stat-value {
      color: var(--gold-light);
      font-size: 23px;
      font-weight: 800;
      margin-bottom: 7px;
    }

    .stat-label {
      color: #777;
      font-size: 12px;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    /* Footer */
    footer {
      border-top: 1px solid rgba(255,255,255,0.06);
      padding: 28px 0;
      color: #666;
      font-size: 12px;
      text-align: center;
    }

    .footer-gold {
      color: var(--gold);
    }

    /* Mobile */
    @media (max-width: 650px) {
      nav {
        height: 70px;
      }

      .network {
        display: none;
      }

      h1 {
        letter-spacing: -3px;
      }

      .hero {
        padding-top: 45px;
      }

      .stats {
        grid-template-columns: 1fr;
      }

      .time-box {
        width: 78px;
        padding: 15px 7px;
      }

      .time-number {
        font-size: 25px;
      }

      .buttons {
        flex-direction: column;
        align-items: stretch;
      }

      .btn {
        width: 100%;
      }
    }
  </style>
</head>

<body>

  <div class="particles">
    <span class="particle"></span>
    <span class="particle"></span>
    <span class="particle"></span>
    <span class="particle"></span>
    <span class="particle"></span>
    <span class="particle"></span>
    <span class="particle"></span>
    <span class="particle"></span>
  </div>

  <div class="container">

    <nav>
      <div class="logo">
        <div class="logo-icon">G</div>
        GOLD
      </div>

      <div class="network">
        BNB Smart Chain
      </div>
    </nav>

    <main class="hero">

      <div>

        <div class="badge">
          <span class="badge-dot"></span>
          PRESALE COMING SOON
        </div>

        <h1>GOLD</h1>

        <p class="subtitle">
          A new digital asset is coming to the
          <span class="highlight">BNB Smart Chain.</span>
          The Gold (GLD) presale is currently being prepared.
          Stay tuned for the official launch.
        </p>

        <div class="countdown-title">
          Presale Launch
        </div>

        <div class="countdown">

          <div class="time-box">
            <span class="time-number" id="days">00</span>
            <span class="time-label">Days</span>
          </div>

          <div class="time-box">
            <span class="time-number" id="hours">00</span>
            <span class="time-label">Hours</span>
          </div>

          <div class="time-box">
            <span class="time-number" id="minutes">00</span>
            <span class="time-label">Minutes</span>
          </div>

          <div class="time-box">
            <span class="time-number" id="seconds">00</span>
            <span class="time-label">Seconds</span>
          </div>

        </div>

        <div class="buttons">
          <a href="#" class="btn btn-primary" onclick="notifyComingSoon(event)">
            Notify Me
          </a>

          <a href="#details" class="btn btn-secondary">
            Learn More
          </a>
        </div>

        <section class="stats" id="details">

          <div class="stat">
            <div class="stat-value">$0.0004</div>
            <div class="stat-label">Presale Price</div>
          </div>

          <div class="stat">
            <div class="stat-value">10B</div>
            <div class="stat-label">Total Supply</div>
          </div>

          <div class="stat">
            <div class="stat-value">$4M</div>
            <div class="stat-label">Initial FDV</div>
          </div>

        </section>

      </div>

    </main>

  </div>

  <footer>
    © 2026 <span class="footer-gold">Gold (GLD)</span>.
    All rights reserved.
  </footer>

  <script>
    /*
      ============================================
      SET YOUR PRESALE LAUNCH DATE HERE
      ============================================

      Example:
      new Date("2026-09-01T12:00:00+00:00")

      Change this to your actual launch date/time.
    */

    const launchDate = new Date("2026-09-01T12:00:00+00:00").getTime();

    function updateCountdown() {
      const now = new Date().getTime();
      const distance = launchDate - now;

      if (distance <= 0) {
        document.getElementById("days").textContent = "00";
        document.getElementById("hours").textContent = "00";
        document.getElementById("minutes").textContent = "00";
        document.getElementById("seconds").textContent = "00";
        return;
      }

      const days = Math.floor(distance / (1000 * 60 * 60 * 24));
      const hours = Math.floor(
        (distance % (1000 * 60 * 60 * 24)) /
        (1000 * 60 * 60)
      );

      const minutes = Math.floor(
        (distance % (1000 * 60 * 60)) /
        (1000 * 60)
      );

      const seconds = Math.floor(
        (distance % (1000 * 60)) /
        1000
      );

      document.getElementById("days").textContent =
        String(days).padStart(2, "0");

      document.getElementById("hours").textContent =
        String(hours).padStart(2, "0");

      document.getElementById("minutes").textContent =
        String(minutes).padStart(2, "0");

      document.getElementById("seconds").textContent =
        String(seconds).padStart(2, "0");
    }

    updateCountdown();
    setInterval(updateCountdown, 1000);

    function notifyComingSoon(event) {
      event.preventDefault();

      alert(
        "The Gold (GLD) presale is coming soon. Please check back for the official launch."
      );
    }
  </script>

</body>
</html>
