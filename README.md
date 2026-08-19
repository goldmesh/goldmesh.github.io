<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Gold — Coming Soon">
  <title>Gold — Coming Soon</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html,
    body {
      width: 100%;
      height: 100%;
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
        Helvetica, Arial, sans-serif;
      background: #050505;
      color: #ffffff;
      overflow: hidden;
    }

    .page {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
      background:
        radial-gradient(
          circle at 50% 45%,
          rgba(212, 175, 55, 0.12),
          transparent 30%
        ),
        #050505;
    }

    /* Ambient glow */
    .glow {
      position: absolute;
      width: 500px;
      height: 500px;
      border-radius: 50%;
      background: rgba(212, 175, 55, 0.08);
      filter: blur(100px);
      pointer-events: none;
    }

    /* Decorative circles */
    .circle {
      position: absolute;
      border: 1px solid rgba(212, 175, 55, 0.08);
      border-radius: 50%;
      pointer-events: none;
    }

    .circle.one {
      width: 700px;
      height: 700px;
    }

    .circle.two {
      width: 950px;
      height: 950px;
      border-color: rgba(212, 175, 55, 0.045);
    }

    .content {
      position: relative;
      z-index: 2;
      text-align: center;
      padding: 30px;
    }

    .logo {
      width: 74px;
      height: 74px;
      margin: 0 auto 30px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;

      background: linear-gradient(
        145deg,
        #f7dc72,
        #d4af37 50%,
        #92751c
      );

      color: #080808;
      font-size: 32px;
      font-weight: 900;

      box-shadow:
        0 0 30px rgba(212, 175, 55, 0.18),
        inset 0 1px 2px rgba(255, 255, 255, 0.4);
    }

    .brand {
      font-size: 15px;
      font-weight: 700;
      letter-spacing: 7px;
      color: #d4af37;
      margin-left: 7px;
      text-transform: uppercase;
      margin-bottom: 22px;
    }

    h1 {
      font-size: clamp(48px, 8vw, 88px);
      line-height: 1;
      font-weight: 800;
      letter-spacing: -3px;
      margin-bottom: 22px;

      background: linear-gradient(
        135deg,
        #ffffff 20%,
        #f5d76e 55%,
        #a88420
      );

      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }

    .subtitle {
      color: #888888;
      font-size: 17px;
      letter-spacing: 0.3px;
      line-height: 1.7;
      max-width: 520px;
      margin: 0 auto;
    }

    .line {
      width: 55px;
      height: 1px;
      margin: 34px auto 0;
      background: linear-gradient(
        90deg,
        transparent,
        #d4af37,
        transparent
      );
    }

    footer {
      position: absolute;
      bottom: 25px;
      left: 0;
      width: 100%;
      text-align: center;
      color: #444444;
      font-size: 11px;
      letter-spacing: 1px;
      z-index: 2;
    }

    @media (max-width: 600px) {
      .logo {
        width: 64px;
        height: 64px;
        font-size: 27px;
      }

      .brand {
        font-size: 13px;
        letter-spacing: 5px;
      }

      h1 {
        letter-spacing: -2px;
      }

      .subtitle {
        font-size: 15px;
      }

      .circle.one {
        width: 500px;
        height: 500px;
      }

      .circle.two {
        width: 700px;
        height: 700px;
      }
    }
  </style>
</head>

<body>

  <main class="page">

    <div class="glow"></div>

    <div class="circle one"></div>
    <div class="circle two"></div>

    <div class="content">

      <div class="logo">G</div>

      <div class="brand">Gold</div>

      <h1>Coming Soon</h1>

      <p class="subtitle">
        Something new is being built.
        <br>
        Stay tuned.
      </p>

      <div class="line"></div>

    </div>

    <footer>
      © 2026 Gold. All rights reserved.
    </footer>

  </main>

</body>
</html>
