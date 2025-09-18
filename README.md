<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>KEROFROG — The Frog Memecoin</title>
  <link href="https://fonts.googleapis.com/css2?family=Luckiest+Guy&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Luckiest Guy', cursive, sans-serif;
      background: linear-gradient(to bottom, #f7f6c5, #e1df7c, #c2b83b);
      color: #2a2a2a;
      line-height: 1.6;
      text-align: center;
    }

    h3 {
      font-size: 2rem;
      margin: 40px 0 20px;
    }

    section {
      padding: 40px 20px;
    }

    .card {
      background: #fff8b0;
      border-radius: 16px;
      padding: 20px;
      max-width: 280px;
      text-align: center;
      box-shadow: 0 6px 12px rgba(0,0,0,0.2);
      transition: all 0.6s ease-out;
      opacity: 0;
      transform: translateY(50px);
    }

    .card img {
      max-width: 100%;
      border-radius: 12px;
    }

    .card.show {
      opacity: 1;
      transform: translateY(0);
    }

    /* Lore Section (swamp yellow fog) */
    #lore {
      position: relative;
      background: linear-gradient(to bottom, #e9e26c, #c4bc3f, #9b922a);
      color: #2a2a2a;
      overflow: hidden;
    }

    #lore::before, 
    #lore::after {
      content: "";
      position: absolute;
      top: 0;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle, rgba(255,255,200,0.15) 0%, transparent 70%);
      animation: fogMove 80s linear infinite;
      pointer-events: none;
      filter: blur(70px);
    }

    #lore::after {
      animation-direction: reverse;
      opacity: 0.6;
    }

    /* Frog Jump Animation */
    .frog-jump {
      position: relative;
      margin-top: 40px;
    }

    .frog-jump img {
      width: 80px;
      animation: jump 2s infinite ease-in-out, moveX 6s infinite linear alternate;
    }

    @keyframes jump {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-40px); }
    }

    @keyframes moveX {
      0% { transform: translateX(-40px); }
      100% { transform: translateX(40px); }
    }

    /* Footer */
    footer {
      padding: 30px 10px;
      background: #9c9228;
      font-size: 0.9rem;
      color: #fff;
    }

    footer a {
      color: #fff5a8;
      text-decoration: none;
      margin: 0 8px;
      transition: color 0.3s;
    }

    footer a:hover {
      color: #ffe97d;
    }

    /* Sound Toggle Button */
    #soundToggle {
      background: #ffd84d;
      color: #2a2a2a;
      border: none;
      padding: 10px 20px;
      margin: 20px auto;
      border-radius: 20px;
      font-size: 1rem;
      cursor: pointer;
      transition: background 0.3s;
    }

    #soundToggle:hover {
      background: #ffe97d;
    }

    /* Fog Animation */
    @keyframes fogMove {
      0% { transform: translateX(0); }
      100% { transform: translateX(50%); }
    }
  </style>
</head>
<body>

  <!-- Lore & Mission -->
  <section id="lore">
    <h3>LORE</h3>
    <p style="max-width:800px; margin:20px auto; font-size:1.2rem;">
      Long ago, deep in the mystical swamps, the Kerofrog was born — a playful spirit of frogs united by memes, laughter, and community power. 
      From simple ripples in the pond to waves across the blockchain, Kerofrog represents fun, freedom, and a leap into the future of memecoins.
    </p>

    <h3>MISSION</h3>
    <p style="max-width:800px; margin:20px auto; font-size:1.2rem;">
      Our mission is simple: spread joy, build a strong community, and show that even the smallest frog can make the biggest splash in DeFi.
    </p>

    <!-- Frog Animation -->
    <div class="frog-jump">
      <img src="https://raw.githubusercontent.com/Rudip5131/froggalery/refs/heads/main/frog.jpeg" alt="Jumping Frog" />
    </div>

    <!-- Toggle Button -->
    <button id="soundToggle">🔊 Sound ON</button>
    <audio id="bg-audio" loop>
      <source src="https://cdn.pixabay.com/download/audio/2021/09/07/audio_94c7b9b2a4.mp3?filename=forest-crickets-ambient-6232.mp3" type="audio/mpeg">
    </audio>
  </section>

  <!-- NFT Gallery -->
  <section id="nft-gallery">
    <h3>KEROFROG NFT GALLERY</h3>
    <div style="display:flex; flex-wrap:wrap; justify-content:center; gap:20px; max-width:1200px; margin:0 auto;">
      <div class="card">
        <img src="https://raw.githubusercontent.com/Rudip5131/froggalery/refs/heads/main/frog.jpeg" alt="KEROFROG NFT Artwork #1" />
      </div>
      <div class="card">
        <img src="https://raw.githubusercontent.com/Rudip5131/froggalery/refs/heads/main/frog.jpeg" alt="KEROFROG NFT Artwork #2" />
      </div>
      <div class="card">
        <img src="https://raw.githubusercontent.com/Rudip5131/froggalery/refs/heads/main/frog.jpeg" alt="KEROFROG NFT Artwork #3" />
      </div>
    </div>
  </section>

  <!-- How to Buy -->
  <section id="how-to-buy">
    <h3>HOW TO BUY</h3>
    <div style="display:flex; flex-wrap:wrap; justify-content:center; gap:20px; max-width:1200px; margin:0 auto 60px auto;">
      <div class="card">
        <h4>Step 1</h4>
        <p>
          Download 
          <a href="https://play.google.com/store/apps/details?id=com.starkey.wallet" target="_blank" style="color:#2a2a2a; text-decoration:underline; font-weight:bold;">
          Starkey Wallet</a> from the Play Store / Chrome extension.
        </p>
      </div>
      <div class="card">
        <h4>Step 2</h4>
        <p>Top up your Starkey Wallet with Supra.</p>
      </div>
      <div class="card">
        <h4>Step 3</h4>
        <p>
          Connect your wallet to 
          <a href="https://pumpit.pro" target="_blank" style="color:#2a2a2a; text-decoration:underline; font-weight:bold;">
          PUMPIT</a>.
        </p>
      </div>
      <div class="card">
        <h4>Step 4</h4>
        <p>Swap your Supra for <strong>FROG</strong> tokens.</p>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    © 2025 KEROFROG Memecoin. All Rights Reserved. <br />
    <a href="https://twitter.com/kerofrogl" target="_blank">Twitter</a> | 
    <a href="https://t.me/Kerofrogsup" target="_blank">Telegram</a>
  </footer>

  <script>
    // Show cards with animation on scroll
    const cards = document.querySelectorAll('.card');
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if(entry.isIntersecting){
          entry.target.classList.add('show');
        }
      });
    }, { threshold: 0.2 });
    cards.forEach(card => observer.observe(card));

    // Sound Toggle
    const soundToggle = document.getElementById("soundToggle");
    const bgAudio = document.getElementById("bg-audio");
    let isPlaying = false;

    soundToggle.addEventListener("click", () => {
      if (isPlaying) {
        bgAudio.pause();
        soundToggle.textContent = "🔇 Sound OFF";
      } else {
        bgAudio.play();
        soundToggle.textContent = "🔊 Sound ON";
      }
      isPlaying = !isPlaying;
    });
  </script>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/anchor-js/4.1.0/anchor.min.js" 
    integrity="sha256-lZaRhKri35AyJSypXXs4o6OPFTbTmUoltBbDCbdzegg=" crossorigin="anonymous"></script>
  <script>anchors.add();</script>

</body>
</html>
