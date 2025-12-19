---
title: Welcome to Knowledge Tree
---

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Knowledge Tree — Welcome</title>
  <meta name="description" content="Welcome to Knowledge Tree — a personal catalog of topics across science, history, religion, technology, art, and more." />

  <style>
    :root{
      --bg: #0b0d10;
      --panel: #0f141a;
      --text: #e8eef6;
      --muted: #a9b6c7;
      --border: rgba(255,255,255,.10);
      --shadow: 0 10px 30px rgba(0,0,0,.45);
      --radius: 18px;
      --max: 980px;
    }

    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";
      background: radial-gradient(1100px 700px at 20% -10%, rgba(110,168,254,.20), transparent 60%),
                  radial-gradient(900px 600px at 90% 0%, rgba(34,211,238,.16), transparent 55%),
                  var(--bg);
      color: var(--text);
      line-height: 1.6;
    }

    a { color: inherit; }
    .wrap { max-width: var(--max); margin: 0 auto; padding: 28px 18px 70px; }

    .hero {
      border: 1px solid var(--border);
      background: linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.03));
      border-radius: calc(var(--radius) + 6px);
      overflow: hidden;
      box-shadow: var(--shadow);
    }

    .hero-top {
      position: relative;
      height: 240px;
      background: #10151c;
    }
    .hero-top img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      display: block;
      filter: saturate(1.05) contrast(1.05);
      opacity: .95;
    }
    .hero-top::after{
      content:"";
      position:absolute; inset:0;
      background: linear-gradient(180deg, rgba(11,13,16,.20), rgba(11,13,16,.88));
    }
    .hero-title {
      position: absolute;
      left: 22px; bottom: 18px;
      z-index: 2;
    }
    .hero-title h1 {
      margin: 0;
      font-size: 2rem;
      letter-spacing: .2px;
    }
    .hero-title p {
      margin: 6px 0 0;
      color: var(--muted);
      max-width: 56ch;
    }

    .content {
      padding: 26px 22px 20px;
    }

    h2 {
      margin: 0 0 12px;
      font-size: 1.35rem;
      letter-spacing: .2px;
    }

    .letter {
      background: rgba(0,0,0,.18);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 18px 18px;
    }

    .letter p { margin: 0 0 12px; color: var(--text); }
    .letter p:last-child { margin-bottom: 0; }
    .signature { margin-top: 14px; color: var(--muted); }

    .grid {
      margin-top: 18px;
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 12px;
    }

    .card {
      border: 1px solid var(--border);
      border-radius: var(--radius);
      overflow: hidden;
      background: rgba(255,255,255,.03);
      box-shadow: 0 8px 18px rgba(0,0,0,.30);
    }
    .card img {
      width: 100%;
      height: 130px;
      object-fit: cover;
      display: block;
    }
    .card .label {
      padding: 10px 12px 12px;
      font-size: .95rem;
      color: var(--muted);
    }

    .footer-note {
      margin-top: 18px;
      color: var(--muted);
      font-size: .95rem;
      border-top: 1px solid var(--border);
      padding-top: 14px;
    }

    @media (max-width: 820px) {
      .hero-top { height: 200px; }
      .grid { grid-template-columns: 1fr; }
      .card img { height: 160px; }
    }
  </style>
</head>

<body>
  <main class="wrap">
    <section class="hero">
      <!-- Put your header image here -->
      <div class="hero-top">
        <img src="assets/hero-knowledge-tree.jpg" alt="Knowledge Tree header image">
        <div class="hero-title">
          <h1>Knowledge Tree</h1>
          <p>A living catalog of whatever I’m curious about — updated often.</p>
        </div>
      </div>

      <div class="content">
        <h2>Welcome Letter</h2>

        <div class="letter">
          <p>
            Welcome to Knowledge Tree, where I collect information on everything and anything I find interest in.
            I believe that everything around is important whether it is science, history, religion, technology, art, etc.
            I will catalog everything and anything I happen to find an interest in. The entries get updated almost daily,
            so keep an eye out for that!
          </p>

          <p>
            If you are interested in specific topics, I am going to work on a way to communicate with me and I can make them priorities!
          </p>

          <p>
            I hope whoever stumbles onto this website, enjoys what they find.
          </p>

          <p class="signature">
            Sincerely,<br />
            The Author
          </p>
        </div>

        <!-- Optional topic image tiles -->
        <div class="grid" aria-label="Featured topics">
          <div class="card">
            <img src="assets/topic-science.jpg" alt="Science">
            <div class="label">Science</div>
          </div>
          <div class="card">
            <img src="assets/topic-history.jpg" alt="History">
            <div class="label">History</div>
          </div>
          <div class="card">
            <img src="assets/topic-art.jpg" alt="Art">
            <div class="label">Art</div>
          </div>
        </div>

        <div class="footer-note">
          <strong>Image directory:</strong> put images in <code>assets/</code> next to this HTML file (or adjust the <code>src</code> paths).
        </div>
      </div>
    </section>
  </main>
</body>
</html>