<!DOCTYPE html>
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
      background: #0a0f0d;
      color: #fff;
      line-height: 1.6;
      text-align: center;
    }

    h3 {
      font-size: 2rem;
      margin: 40px 0 20px;
    }

    section {
      padding: 40px 20px;
      position: relative;
      overflow: hidden;
    }

    .card {
      background: #1b1f1d;
      border-radius: 16px;
      padding: 20px;
      max-width: 280px;
      text-align: center;
      box-shadow: 0 6px 12px rgba(0,0,0,0.3);
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

    footer {
      padding: 30px 10px;
      background: #111;
      font-size: 0.9rem;
    }

    footer a {
      color: #4ade80;
      text-decoration: none;
      margin: 0 8px;
      transition: color 0.3s;
    }

    footer a:hover {
      color: #a3e635;
    }

    /* Swamp Background + Fog Effect */
    #lore {
      background: linear-gradient(to bottom, #0f1f0f, #142814, #0a1a0a);
      color: #d4f7d4;
    }

    #lore::before, 
    #lore::after {
      content: "";
      position: absolute;
      top: 0;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle, rgba(255,255,255,0.07) 0%, transparent 70%);
      animation: fogMove 60s linear infinite;
      pointer-events: none;
      filter: blur(60px);
    }

    #lore::after {
      animation-direction: reverse;
      opacity: 0.6;
    }

    @keyframes fogMove {
      from { transform: translateX(0); }
      to { transform: translateX(200px); }
    }

    /* Frog Jump Animation */
    .frog-jump {
      margin-top: 30px;
    }

    .frog-jump img {
      width: 80px;
      animation: jumpAround 3s infinite ease-in-out;
    }

    @keyframes jumpAround {
      0%   { transform: translate(0, 0) scale(1); }
      20%  { transform: translate(20px, -40px) scale(1.05); }
      40%  { transform: translate(40px, 0) scale(1); }
      60%  { transform: translate(-20px, -40px) scale(1.05); }
      80%  { transform: translate(-40px, 0) scale(1); }
      100% { transform: translate(0, 0) scale(1); }
    }

    /* Toggle Sound Button */
    #sound-toggle {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #1b1f1d;
      border: 2px solid #4ade80;
      color: #4ade80;
      padding: 10px 16px;
      border-radius: 12px;
      font-size: 0.9rem;
      cursor: pointer;
      box-shadow: 0 0 10px rgba(74,222,128,0.6);
      transition: all 0.3s ease;
      z-index: 1000;
    }

    #sound-toggle:hover {
      background: #4ade80;
      color: #111;
      box-shadow: 0 0 20px rgba(74,222,128,1);
    }
  </style>
</head>
<body>

  <!-- Ambient Sound -->
  <audio id="ambient-sound" autoplay loop>
    <source src="https://cdn.pixabay.com/download/audio/2021/09/20/audio_4e84e739f2.mp3?filename=forest-crickets-frogs-ambience-5726.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <!-- Toggle Button -->
  <button id="sound-toggle">🔊 Sound ON</button>

  <!-- LORE Section -->
  <section id="lore">
    <h3>LORE</h3>
    <p style="max-width:800px; margin:20px auto; font-size:1.2rem;">
      Long ago, deep in the mystical swamps, the Kerofrog was born — a playful spirit of frogs united by memes, laughter, and community power. 
      From simple ripples in the pond to waves across the blockchain, Kerofrog represents fun, freedom, and a leap into the future of memecoins.
    </p>

    <!-- Frog Animation -->
    <div class="frog-jump">
      <img src="https://raw.githubusercontent.com/Rudip5131/froggalery/refs/heads/main/frog.jpeg" alt="Jumping Frog" />
    </div>
  </section>

  <!-- MISSION Section -->
  <section id="mission">
    <h3>MISSION</h3>
    <p style="max-width:800px; margin:20px auto; font-size:1.2rem;">
      Our mission is simple: spread joy, build a strong community, and show that even the smallest frog can make the biggest splash in DeFi.
    </p>
  </section>

  <!-- NFT Gallery Section -->
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

  <!-- How to Buy Section -->
  <section id="how-to-buy">
    <h3>HOW TO BUY</h3>
    <div style="display:flex; flex-wrap:wrap; justify-content:center; gap:20px; max-width:1200px; margin:0 auto 60px auto;">
      <div class="card">
        <h4>Step 1</h4>
        <p>Download Starkey Wallet from the Play Store / Chrome extension.</p>
      </div>
      <div class="card">
        <h4>Step 2</h4>
        <p>Top up your Starkey Wallet with Supra.</p>
      </div>
      <div class="card">
        <h4>Step 3</h4>
        <p>Connect your wallet to the PUMPIT.</p>
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

    // Toggle Sound Button
    const audio = document.getElementById('ambient-sound');
    const btn = document.getElementById('sound-toggle');
    btn.addEventListener('click', () => {
      if(audio.paused){
        audio.play();
        btn.textContent = "🔊 Sound ON";
      } else {
        audio.pause();
        btn.textContent = "🔇 Sound OFF";
      }
    });
  </script>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/anchor-js/4.1.0/anchor.min.js" 
    integrity="sha256-lZaRhKri35AyJSypXXs4o6OPFTbTmUoltBbDCbdzegg=" 
    crossorigin="anonymous"></script>
  <script>anchors.add();</script>

</body>
</html>
