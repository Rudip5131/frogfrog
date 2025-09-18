<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>KEROFROG — The Meme Leap Token</title>
  <meta name="description" content="KEROFROG — The meme leap token. A funny, resilient frog that croaks loud, leaps high, and spreads joy in the crypto pond.">
  <link href="https://fonts.googleapis.com/css2?family=Luckiest+Guy&display=swap" rel="stylesheet">
  <style>
    * { margin:0; padding:0; box-sizing:border-box; scroll-behavior: smooth; }
    body { 
      background: #e6ffe6; 
      color:#083b0d; 
      font-family: 'Luckiest Guy', cursive;
      font-weight: bold;
      overflow-x:hidden; 
      text-shadow: 1px 1px 2px #fff;
    }

    header {
      display:flex; 
      flex-direction: column;
      justify-content:center; 
      align-items:center; 
      padding:60px 50px;
      border-radius: 0 0 20px 20px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.3);
      min-height:260px;
      background: linear-gradient(135deg, #9ef01a, #38b000);
    }
    header img {
      width:250px;
      max-width:80%;
      margin-top:20px;
      border-radius:15px;
      box-shadow:0 5px 15px rgba(0,0,0,0.3);
    }
    header h1 {
      color:#042a09;
      font-size:40px;
      margin-top:20px;
      text-shadow:2px 2px 0px #b7e4c7;
    }

    section { padding:60px 20px; }
    .story, .mission {
      max-width:900px; 
      margin:0 auto 60px auto; 
      background: #caffbf; 
      padding:40px; 
      border-radius:25px; 
      line-height:1.9;
      font-size:22px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      text-align:center;
    }

    h3 {
      font-family: 'Luckiest Guy', cursive;
      color:#1a6600;
      margin-bottom:20px;
    }

    .card {
      background: #caffbf;
      border-radius:20px; 
      width:300px;
      height:300px;
      text-align:center; 
      font-size:20px;
      font-weight:bold;
      position:relative; 
      overflow:hidden;
      transition: transform 0.5s, box-shadow 0.5s, opacity 0.8s;
      opacity:0;
      display:flex;
      flex-direction:column;
      justify-content:center;
      align-items:center;
    }
    .card img {
      width:100%;
      height:100%; 
      object-fit: cover; 
      border-radius:15px; 
      transition: transform 0.3s;
    }
    .card:hover img { transform: scale(1.1); }

    .overlay { position:absolute; top:0; left:0; width:100%; height:100%; background: rgba(0,128,0,0.25); opacity:0; transition: opacity 0.3s; border-radius:20px; }
    .card:hover .overlay { opacity:1; }

    .slider-container { position:relative; width:100%; overflow:hidden; margin-bottom:60px; }
    .slider { display:flex; gap:20px; transition: transform 0.5s ease; overflow-x:auto; scroll-behavior: smooth; padding-bottom:10px; }
    .slider::-webkit-scrollbar { display:none; }

    #how-to-buy { text-align:center; }
    #how-to-buy h3 { margin-bottom:40px; }
    #how-to-buy .card { font-size:18px; line-height:1.6; padding:25px; margin:auto; height:auto; }
    #how-to-buy h4 { font-size:24px; margin-bottom:10px; color:#1a6600; }

    footer { 
      background: #70e000;
      text-align:center; 
      padding:35px; 
      border-radius:20px 20px 0 0; 
      color:#042a09; 
      letter-spacing:2px; 
      font-size:18px;
    }
    footer a {
      color:#064d1f;
      text-decoration:none;
      margin: 0 10px;
    }
    footer a:hover { text-decoration:underline; }

    @media (max-width:768px){
      .story, .mission { font-size:20px; padding:30px; }
      .card { width:90%; height:auto; margin-bottom:20px; }
      header img { width:200px; }
      header h1 { font-size:32px; }
    }
    @media (max-width:480px){
      .story, .mission { font-size:18px; padding:20px; }
      #how-to-buy h4 { font-size:20px; }
      header img { width:150px; }
      header h1 { font-size:26px; }
    }
  </style>
</head>
<body>

<header>
  <img src="https://raw.githubusercontent.com/Rudip5131/Pigo-gallery/refs/heads/main/kerofrog.png" alt="KEROFROG Logo">
  <h1>KEROFROG</h1>
</header>

<section class="hero">
  <div class="story">
    <h3>LORE</h3>
    <p>Deep in the swamp, there was one frog whose croak went <strong>“KERO KERO”</strong> louder than all the others. The pond laughed, thinking he was silly.</p>
    <p>But KEROFROG kept leaping, croaking, and dancing until the whole pond started to follow. What was once mocked became a movement.</p>
    <p>KEROFROG rose from the mud as the meme frog of destiny — spreading joy, chaos, and green vibes across the crypto pond.</p>
  </div>
</section>

<section class="mission">
  <h3>MISSION</h3>
  <p><strong>Mission:</strong> To create a fun, unstoppable frog movement that unites memecoin lovers everywhere. We leap higher, croak louder, and spread laughter louder than FUD.</p>
  <p>KEROFROG isn’t just a token — it’s a leap of faith into the wild world of memes and community.</p>
</section>

<section id="gallery">
  <h3>GALLERY</h3>
  <div class="slider-container">
    <div class="slider">
      <div class="card"><img src="https://raw.githubusercontent.com/Rudip5131/Pigo-gallery/refs/heads/main/kerofrog1.png" alt="KEROFROG NFT 1"><div class="overlay"></div></div>
      <div class="card"><img src="https://raw.githubusercontent.com/Rudip5131/Pigo-gallery/refs/heads/main/kerofrog2.png" alt="KEROFROG NFT 2"><div class="overlay"></div></div>
      <div class="card"><img src="https://raw.githubusercontent.com/Rudip5131/Pigo-gallery/refs/heads/main/kerofrog3.png" alt="KEROFROG NFT 3"><div class="overlay"></div></div>
    </div>
  </div>
</section>

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
      <p>Connect your wallet to the DEX.</p>
    </div>
    <div class="card">
      <h4>Step 4</h4>
      <p>Swap your Supra for <strong>KEROFROG</strong> tokens.</p>
    </div>
  </div>
</section>

<footer>
  © 2025 KEROFROG Memecoin. All Rights Reserved. <br>
  <a href="https://twitter.com/kerofrog" target="_blank">Twitter</a> | 
  <a href="https://t.me/kerofrog" target="_blank">Telegram</a>
</footer>

<script>
  // Show cards with animation on scroll
  const cards = document.querySelectorAll('.card');
  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if(entry.isIntersecting){
        entry.target.style.opacity = "1";
        entry.target.style.transform = "translateY(0)";
      }
    });
  }, { threshold: 0.2 });
  cards.forEach(card => {
    card.style.transform = "translateY(50px)";
    observer.observe(card);
  });
</script>

</body>
</html>
