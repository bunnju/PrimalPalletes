<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Primal Palettes</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #111;
      color: #f1f1f1;
      margin: 0;
      padding: 20px;
    }

    .discord-button {
      display: inline-block;
      background-color: #5865F2;
      color: white;
      padding: 10px 20px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
      margin: 10px;
      transition: background 0.3s ease;
    }

    .discord-button:hover {
      background-color: #4752C4;
    }

    header {
      text-align: center;
      margin-bottom: 30px;
    }

    .navbar {
      margin-top: 10px;
    }

    .navbar button {
      background: #333;
      color: #fff;
      border: none;
      margin: 5px;
      padding: 10px 15px;
      border-radius: 5px;
      cursor: pointer;
    }

    .navbar button:hover {
      background: #555;
    }

    .skin-card {
      background: #222;
      border-radius: 10px;
      padding: 20px;
      margin: 20px auto;
      max-width: 1200px;
      display: block;
    }

    .skin-card img {
      max-width: 100%;
      border-radius: 5px;
      margin: 10px 0;
    }

    footer {
      border-top: 1px solid #333;
      background-color: #0f0f0f;
      color: #999;
      padding: 20px;
      font-size: 0.9rem;
      text-align: center;
    }

    footer strong {
      color: #ccc;
    }

    .notice-box {
      background-color: #222;
      border-left: 4px solid #f39c12;
      padding: 15px;
      margin: 20px auto;
      max-width: 800px;
      border-radius: 5px;
      color: #f1c40f;
      font-size: 1rem;
    }

    .notice-box strong {
      color: #f9e79f;
    }
  </style>
</head>
<body>
  <header>
    <h1>Primal Palettes</h1>
    <h4>By <i>Bunnju</i></h4>
    <p>
      These are all my skins that are for sale.<br />
      I make them for the unofficial Isle server called Primal Heaven!<br />
      <a href="https://discord.gg/ckgyXEKp" class="discord-button" target="_blank">
        Join the fun here!
      </a>
    </p>

    <div class="notice-box">
      <strong>⚠️ Info:</strong> All skins are designed using the <strong>male version</strong> of each dinosaur. To see the intended appearance in-game, please use a <strong>male dino</strong>!
    </div>

    <nav class="navbar">
      <button data-category="all">All</button>
      <button data-category="glitter">Glitter</button>
      <button data-category="glitch">Glitch</button>
      <button data-category="normal">Normal</button>
    </nav>
  </header>

  <main id="skin-container" style="text-align:center;">
    <!-- Add your skin cards here like you've already done -->
    <!-- Example skin card (keep using the format you already have) -->
    <section class="skin-card glitter">
      <h2>Example Skin</h2>
      <div style="text-align: center; margin: 20px; font-size: 1.1rem;">
        <img src="https://i.gifer.com/origin/e0/e02ce86bcfd6d1d6c2f775afb3ec8c01_w200.gif" style="width:34px; vertical-align: middle;">
        <strong>5,000 PP</strong>
        <img src="https://i.gifer.com/origin/e0/e02ce86bcfd6d1d6c2f775afb3ec8c01_w200.gif" style="width:34px; vertical-align: middle;">
      </div>
      <img src="https://via.placeholder.com/800x300" alt="Skin preview">
    </section>
  </main>

  <footer>
    <p><strong>Disclaimer:</strong> All skins shown here are fan-made content created by <i>Bunnju</i> for the unofficial Isle server <strong>Primal Heaven</strong>. This site is not affiliated with or endorsed by <em>The Isle</em> or its developers.</p>
  </footer>

  <script>
    const buttons = document.querySelectorAll('nav button');
    const cards = document.querySelectorAll('.skin-card');

    buttons.forEach(button => {
      button.addEventListener('click', () => {
        const category = button.getAttribute('data-category');
        cards.forEach(card => {
          if (category === 'all' || card.classList.contains(category)) {
            card.style.display = 'block';
          } else {
            card.style.display = 'none';
          }
        });
      });
    });
  </script>
</body>
</html>
