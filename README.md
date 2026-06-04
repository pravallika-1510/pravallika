<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Pravalika 💖</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;0,900;1,400&family=Quicksand:wght@300;400;600&display=swap" rel="stylesheet">
<style>
  :root {
    --pink: #ff3d7f;
    --rose: #ff6b9d;
    --gold: #ffd700;
    --purple: #9b59b6;
    --deep: #1a0a2e;
    --light: #fff0f7;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    background: var(--deep);
    font-family: 'Quicksand', sans-serif;
    overflow-x: hidden;
    cursor: none;
  }

  /* Custom cursor */
  .cursor {
    width: 20px; height: 20px;
    background: var(--pink);
    border-radius: 50%;
    position: fixed;
    pointer-events: none;
    z-index: 99999;
    transform: translate(-50%, -50%);
    transition: transform 0.1s, width 0.2s, height 0.2s;
    mix-blend-mode: screen;
  }

  /* Floating particles */
  .particles {
    position: fixed;
    width: 100%; height: 100%;
    pointer-events: none;
    z-index: 0;
    overflow: hidden;
  }

  .particle {
    position: absolute;
    bottom: -50px;
    font-size: 18px;
    animation: floatUp linear infinite;
    opacity: 0;
  }

  @keyframes floatUp {
    0% { transform: translateY(0) rotate(0deg); opacity: 1; }
    100% { transform: translateY(-110vh) rotate(720deg); opacity: 0; }
  }

  /* Pages */
  .page {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 40px 20px;
    position: relative;
    z-index: 1;
  }

  .hidden { display: none !important; }

  /* ===== PAGE 1 - WELCOME ===== */
  #welcome {
    background: radial-gradient(ellipse at center, #2d0a4e 0%, #1a0a2e 70%);
  }

  .welcome-bg {
    position: absolute;
    width: 100%; height: 100%;
    overflow: hidden;
  }

  .star {
    position: absolute;
    background: white;
    border-radius: 50%;
    animation: twinkle ease-in-out infinite;
  }

  @keyframes twinkle {
    0%, 100% { opacity: 0.2; transform: scale(1); }
    50% { opacity: 1; transform: scale(1.5); }
  }

  .welcome-content {
    text-align: center;
    z-index: 2;
  }

  .crown {
    font-size: 5rem;
    animation: bounce 2s ease-in-out infinite;
    display: block;
    margin-bottom: 10px;
  }

  @keyframes bounce {
    0%, 100% { transform: translateY(0) rotate(-5deg); }
    50% { transform: translateY(-15px) rotate(5deg); }
  }

  .welcome-title {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2.5rem, 8vw, 5rem);
    font-weight: 900;
    background: linear-gradient(135deg, #ff3d7f, #ffd700, #ff6b9d, #fff);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    line-height: 1.1;
    text-shadow: none;
    animation: shimmer 3s ease-in-out infinite;
    background-size: 200% 200%;
  }

  @keyframes shimmer {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  .welcome-name {
    font-family: 'Playfair Display', serif;
    font-size: clamp(3rem, 10vw, 7rem);
    font-weight: 900;
    font-style: italic;
    color: var(--gold);
    text-shadow: 0 0 30px rgba(255,215,0,0.5), 0 0 60px rgba(255,215,0,0.3);
    animation: glow 2s ease-in-out infinite;
  }

  @keyframes glow {
    0%, 100% { text-shadow: 0 0 30px rgba(255,215,0,0.5); }
    50% { text-shadow: 0 0 60px rgba(255,215,0,0.9), 0 0 100px rgba(255,215,0,0.5); }
  }

  .welcome-sub {
    color: rgba(255,255,255,0.7);
    font-size: 1.1rem;
    margin: 20px 0 40px;
    letter-spacing: 3px;
    text-transform: uppercase;
  }

  .btn-main {
    padding: 18px 50px;
    border: none;
    border-radius: 50px;
    background: linear-gradient(135deg, var(--pink), var(--purple));
    color: white;
    font-size: 1.1rem;
    font-family: 'Quicksand', sans-serif;
    font-weight: 600;
    cursor: pointer;
    letter-spacing: 2px;
    text-transform: uppercase;
    box-shadow: 0 10px 40px rgba(255,61,127,0.4), 0 0 0 0 rgba(255,61,127,0.4);
    animation: pulse-btn 2s ease-in-out infinite;
    transition: transform 0.2s;
  }

  .btn-main:hover { transform: scale(1.05); }

  @keyframes pulse-btn {
    0%, 100% { box-shadow: 0 10px 40px rgba(255,61,127,0.4), 0 0 0 0 rgba(255,61,127,0.4); }
    50% { box-shadow: 0 10px 40px rgba(255,61,127,0.6), 0 0 0 15px rgba(255,61,127,0); }
  }

  /* ===== PAGE 2 - ENVELOPE ===== */
  #envelopePage {
    background: radial-gradient(ellipse at center, #3d0a5e 0%, #1a0a2e 70%);
  }

  .envelope-wrap {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 30px;
  }

  .env-title {
    font-family: 'Playfair Display', serif;
    color: white;
    font-size: 1.8rem;
    text-align: center;
  }

  .envelope {
    width: 300px;
    height: 200px;
    position: relative;
    cursor: pointer;
    filter: drop-shadow(0 20px 40px rgba(255,61,127,0.5));
    transition: transform 0.3s;
    animation: envFloat 3s ease-in-out infinite;
  }

  @keyframes envFloat {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-15px); }
  }

  .envelope:hover { transform: scale(1.05) translateY(-5px); }

  .env-body {
    width: 100%; height: 100%;
    background: linear-gradient(135deg, #ff3d7f, #9b59b6);
    border-radius: 10px;
    position: relative;
    overflow: hidden;
  }

  .env-flap {
    position: absolute;
    top: 0; left: 0;
    width: 100%; height: 55%;
    background: linear-gradient(135deg, #ff6b9d, #c0399e);
    clip-path: polygon(0 0, 100% 0, 50% 100%);
    z-index: 2;
  }

  .env-bottom {
    position: absolute;
    bottom: 0; left: 0;
    width: 100%; height: 55%;
    background: linear-gradient(135deg, #d63083, #8e44ad);
    clip-path: polygon(0 100%, 100% 100%, 50% 0%);
  }

  .env-left {
    position: absolute;
    top: 0; left: 0;
    width: 50%; height: 100%;
    background: rgba(0,0,0,0.1);
    clip-path: polygon(0 0, 100% 50%, 0 100%);
  }

  .env-right {
    position: absolute;
    top: 0; right: 0;
    width: 50%; height: 100%;
    background: rgba(255,255,255,0.1);
    clip-path: polygon(100% 0, 0 50%, 100% 100%);
  }

  .env-heart {
    position: absolute;
    top: 50%; left: 50%;
    transform: translate(-50%, -50%);
    font-size: 3rem;
    z-index: 3;
    animation: heartbeat 1.2s ease-in-out infinite;
  }

  @keyframes heartbeat {
    0%, 100% { transform: translate(-50%, -50%) scale(1); }
    50% { transform: translate(-50%, -50%) scale(1.2); }
  }

  .tap-hint {
    color: rgba(255,255,255,0.6);
    font-size: 0.9rem;
    letter-spacing: 2px;
    text-transform: uppercase;
    animation: blink 1.5s ease-in-out infinite;
  }

  @keyframes blink {
    0%, 100% { opacity: 0.4; }
    50% { opacity: 1; }
  }

  /* ===== PAGE 3 - ALBUM ===== */
  #albumPage {
    background: linear-gradient(135deg, #1a0a2e, #2d0a4e, #1a0a2e);
  }

  .album-title {
    font-family: 'Playfair Display', serif;
    font-size: 2rem;
    color: var(--gold);
    text-align: center;
    margin-bottom: 30px;
    letter-spacing: 2px;
  }

  .album-frame {
    position: relative;
    width: min(350px, 90vw);
  }

  .album-border {
    position: absolute;
    inset: -8px;
    border-radius: 28px;
    background: linear-gradient(135deg, var(--gold), var(--pink), var(--purple), var(--gold));
    background-size: 300% 300%;
    animation: borderSpin 3s linear infinite;
    z-index: 0;
  }

  @keyframes borderSpin {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  .album-img-wrap {
    position: relative;
    z-index: 1;
    border-radius: 20px;
    overflow: hidden;
    background: #2d0a4e;
  }

  .album-img-wrap img {
    width: 100%;
    height: 420px;
    object-fit: cover;
    display: block;
    transition: transform 0.5s ease;
  }

  .album-img-wrap img:hover { transform: scale(1.03); }

  .photo-overlay {
    position: absolute;
    bottom: 0; left: 0; right: 0;
    padding: 30px 20px 20px;
    background: linear-gradient(transparent, rgba(26,10,46,0.95));
    z-index: 2;
  }

  .caption {
    color: white;
    font-size: 1rem;
    font-style: italic;
    text-align: center;
    line-height: 1.5;
  }

  .slide-counter {
    color: var(--gold);
    font-size: 0.85rem;
    text-align: center;
    margin-top: 5px;
    letter-spacing: 2px;
  }

  .controls {
    display: flex;
    gap: 20px;
    margin-top: 25px;
    align-items: center;
  }

  .btn-arrow {
    width: 55px; height: 55px;
    border-radius: 50%;
    border: 2px solid var(--pink);
    background: rgba(255,61,127,0.1);
    color: white;
    font-size: 1.3rem;
    cursor: pointer;
    transition: all 0.3s;
    backdrop-filter: blur(10px);
  }

  .btn-arrow:hover {
    background: var(--pink);
    transform: scale(1.1);
    box-shadow: 0 0 20px rgba(255,61,127,0.5);
  }

  .dots {
    display: flex;
    gap: 8px;
  }

  .dot {
    width: 8px; height: 8px;
    border-radius: 50%;
    background: rgba(255,255,255,0.3);
    transition: all 0.3s;
    cursor: pointer;
  }

  .dot.active {
    background: var(--pink);
    width: 24px;
    border-radius: 4px;
    box-shadow: 0 0 10px var(--pink);
  }

  .btn-letter {
    margin-top: 30px;
    padding: 15px 40px;
    border: 2px solid var(--gold);
    border-radius: 50px;
    background: transparent;
    color: var(--gold);
    font-family: 'Quicksand', sans-serif;
    font-size: 1rem;
    font-weight: 600;
    cursor: pointer;
    letter-spacing: 2px;
    text-transform: uppercase;
    transition: all 0.3s;
  }

  .btn-letter:hover {
    background: var(--gold);
    color: var(--deep);
    box-shadow: 0 0 30px rgba(255,215,0,0.4);
  }

  /* ===== PAGE 4 - LETTER ===== */
  #letterPage {
    background: radial-gradient(ellipse at top, #3d0a5e 0%, #1a0a2e 60%);
  }

  .letter-outer {
    max-width: 680px;
    width: 95%;
    position: relative;
  }

  .letter-decoration {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 10px;
    animation: spinSlow 8s linear infinite;
  }

  @keyframes spinSlow {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  .letter-card {
    background: rgba(255,255,255,0.05);
    backdrop-filter: blur(20px);
    border: 1px solid rgba(255,215,0,0.2);
    border-radius: 30px;
    padding: 50px 40px;
    position: relative;
    overflow: hidden;
  }

  .letter-card::before {
    content: '';
    position: absolute;
    top: -50%; left: -50%;
    width: 200%; height: 200%;
    background: radial-gradient(circle, rgba(255,61,127,0.05) 0%, transparent 60%);
    animation: rotateBg 10s linear infinite;
  }

  @keyframes rotateBg {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  .letter-dear {
    font-family: 'Playfair Display', serif;
    font-size: 1.8rem;
    font-style: italic;
    color: var(--gold);
    margin-bottom: 30px;
    position: relative;
    z-index: 1;
  }

  .letter-text {
    color: rgba(255,255,255,0.85);
    line-height: 2;
    font-size: 1.05rem;
    position: relative;
    z-index: 1;
    text-align: left;
  }

  .letter-text .highlight {
    color: var(--rose);
    font-weight: 600;
  }

  .letter-sign {
    margin-top: 35px;
    font-family: 'Playfair Display', serif;
    font-style: italic;
    font-size: 1.3rem;
    color: var(--gold);
    text-align: right;
    position: relative;
    z-index: 1;
  }

  .btn-final {
    margin-top: 30px;
    padding: 18px 50px;
    border: none;
    border-radius: 50px;
    background: linear-gradient(135deg, var(--gold), #ff9f43);
    color: var(--deep);
    font-family: 'Quicksand', sans-serif;
    font-size: 1.1rem;
    font-weight: 700;
    cursor: pointer;
    letter-spacing: 2px;
    text-transform: uppercase;
    box-shadow: 0 10px 30px rgba(255,215,0,0.3);
    transition: all 0.3s;
  }

  .btn-final:hover {
    transform: translateY(-3px);
    box-shadow: 0 15px 40px rgba(255,215,0,0.5);
  }

  /* ===== PAGE 5 - FINAL ===== */
  #finalPage {
    background: radial-gradient(ellipse at center, #2d0a4e 0%, #1a0a2e 70%);
    text-align: center;
  }

  .firework {
    position: absolute;
    width: 100%; height: 100%;
    pointer-events: none;
    overflow: hidden;
  }

  .fw-particle {
    position: absolute;
    width: 6px; height: 6px;
    border-radius: 50%;
    animation: fwExplode ease-out forwards;
  }

  @keyframes fwExplode {
    0% { transform: translate(0, 0) scale(1); opacity: 1; }
    100% { transform: translate(var(--tx), var(--ty)) scale(0); opacity: 0; }
  }

  .final-emoji {
    font-size: 5rem;
    display: block;
    animation: finalBounce 0.8s ease-in-out infinite alternate;
  }

  @keyframes finalBounce {
    0% { transform: translateY(0) scale(1); }
    100% { transform: translateY(-20px) scale(1.1); }
  }

  .final-title {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2.5rem, 8vw, 5rem);
    font-weight: 900;
    background: linear-gradient(135deg, #ffd700, #ff3d7f, #fff, #ffd700);
    background-size: 300% 300%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: shimmer 2s ease-in-out infinite;
    line-height: 1.2;
    margin: 20px 0 10px;
  }

  .final-name {
    font-family: 'Playfair Display', serif;
    font-size: clamp(3rem, 10vw, 7rem);
    font-weight: 900;
    font-style: italic;
    color: var(--gold);
    text-shadow: 0 0 40px rgba(255,215,0,0.6);
    animation: glow 1.5s ease-in-out infinite;
  }

  .final-msg {
    color: rgba(255,255,255,0.8);
    font-size: 1.15rem;
    line-height: 2;
    max-width: 500px;
    margin: 30px auto;
  }

  .final-hearts {
    font-size: 2.5rem;
    animation: finalBounce 1s ease-in-out infinite alternate;
    display: block;
    margin-top: 20px;
  }

  /* Ring of roses decoration */
  .rose-ring {
    position: absolute;
    width: 500px; height: 500px;
    border-radius: 50%;
    animation: rotateSlow 15s linear infinite;
    pointer-events: none;
  }

  @keyframes rotateSlow {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  .rose-item {
    position: absolute;
    font-size: 1.5rem;
    top: 50%; left: 50%;
  }

  /* Music player */
  .music-player {
    position: fixed;
    bottom: 20px;
    right: 20px;
    z-index: 999;
    background: rgba(26,10,46,0.9);
    backdrop-filter: blur(20px);
    border: 1px solid rgba(255,61,127,0.3);
    border-radius: 60px;
    padding: 12px 20px;
    display: flex;
    align-items: center;
    gap: 12px;
    box-shadow: 0 10px 30px rgba(0,0,0,0.3);
  }

  .music-icon {
    font-size: 1.3rem;
    animation: musicPulse 1s ease-in-out infinite;
  }

  @keyframes musicPulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.2); }
  }

  .music-bars {
    display: flex;
    align-items: flex-end;
    gap: 3px;
    height: 20px;
  }

  .bar {
    width: 4px;
    background: var(--pink);
    border-radius: 2px;
    animation: barDance ease-in-out infinite;
  }

  .bar:nth-child(1) { animation-duration: 0.6s; height: 8px; }
  .bar:nth-child(2) { animation-duration: 0.8s; height: 14px; }
  .bar:nth-child(3) { animation-duration: 0.5s; height: 18px; }
  .bar:nth-child(4) { animation-duration: 0.9s; height: 11px; }
  .bar:nth-child(5) { animation-duration: 0.7s; height: 16px; }

  @keyframes barDance {
    0%, 100% { transform: scaleY(0.3); }
    50% { transform: scaleY(1); }
  }

  /* Page transitions */
  .page {
    animation: fadeIn 0.8s ease forwards;
  }

  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  /* Ribbon */
  .ribbon {
    position: absolute;
    top: 20px;
    background: linear-gradient(135deg, var(--pink), var(--purple));
    color: white;
    padding: 8px 30px;
    font-size: 0.8rem;
    letter-spacing: 3px;
    text-transform: uppercase;
    font-weight: 600;
    clip-path: polygon(0 0, calc(100% - 15px) 0, 100% 50%, calc(100% - 15px) 100%, 0 100%, 15px 50%);
  }
</style>
</head>
<body>

<div class="cursor" id="cursor"></div>

<!-- Floating Particles -->
<div class="particles" id="particles"></div>

<!-- Music Player UI -->
<div class="music-player">
  <span class="music-icon">🎵</span>
  <div class="music-bars">
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
  </div>
</div>

<!-- AUDIO - Change the src to your music file -->
<audio id="bgMusic" loop>
  <source src="your-music-file.mp3" type="audio/mpeg">
</audio>

<!-- ===== PAGE 1 - WELCOME ===== -->
<section class="page" id="welcome">
  <div class="welcome-bg" id="starsBg"></div>

  <div class="welcome-content">
    <span class="crown">👑</span>
    <h1 class="welcome-title">Happy Birthday</h1>
    <h1 class="welcome-name">Pravalika</h1>
    <p class="welcome-sub">A special surprise made with love 💖</p>
    <button class="btn-main" onclick="goTo('welcome','envelopePage')">
      Open Your Surprise 🎁
    </button>
  </div>
</section>

<!-- ===== PAGE 2 - ENVELOPE ===== -->
<section class="page hidden" id="envelopePage">
  <div class="envelope-wrap">
    <h2 class="env-title">Something special is waiting for you... 💌</h2>

    <div class="envelope" onclick="goTo('envelopePage','albumPage')">
      <div class="env-body">
        <div class="env-flap"></div>
        <div class="env-bottom"></div>
        <div class="env-left"></div>
        <div class="env-right"></div>
        <div class="env-heart">💌</div>
      </div>
    </div>

    <p class="tap-hint">✨ Tap to open ✨</p>
  </div>
</section>

<!-- ===== PAGE 3 - PHOTO ALBUM ===== -->
<section class="page hidden" id="albumPage">
  <h2 class="album-title">📸 Memory Gallery</h2>

  <div class="album-frame">
    <div class="album-border"></div>
    <div class="album-img-wrap">
      <!-- CHANGE THESE IMAGE SOURCES TO YOUR PHOTOS -->
      <img id="albumImage" src="photo1.jpg" alt="Photo" onerror="this.src='https://via.placeholder.com/350x420/2d0a4e/ff3d7f?text=Your+Photo+Here'">
      <div class="photo-overlay">
        <p class="caption" id="caption">Your beautiful smile lights up every room 🌸</p>
        <p class="slide-counter" id="counter">1 / 5</p>
      </div>
    </div>
  </div>

  <div class="controls">
    <button class="btn-arrow" onclick="prevSlide()">←</button>
    <div class="dots" id="dots"></div>
    <button class="btn-arrow" onclick="nextSlide()">→</button>
  </div>

  <button class="btn-letter" onclick="goTo('albumPage','letterPage')">
    Read My Letter 💌
  </button>
</section>

<!-- ===== PAGE 4 - LETTER ===== -->
<section class="page hidden" id="letterPage">
  <div class="letter-outer">
    <div class="letter-decoration">🌸</div>

    <div class="letter-card">
      <p class="letter-dear">Dear Pravalika,</p>

      <div class="letter-text">
        <p>
          Happy Birthday, my dearest sister! 🎂✨
        </p>
        <br>
        <p>
          Today is not just another day — today is the day the world became a
          <span class="highlight">more beautiful, more joyful, and more magical place</span>
          because you were born into it.
        </p>
        <br>
        <p>
          You have always been the kind of person who brings
          <span class="highlight">light to every room</span> you walk into.
          Your laughter is contagious, your heart is pure,
          and your strength inspires everyone around you.
        </p>
        <br>
        <p>
          Through every storm and every sunshine, you have shown what it truly means to be
          <span class="highlight">graceful, strong, and kind.</span>
          I am so proud to call you my sister.
        </p>
        <br>
        <p>
          On this special day, I wish you a life full of
          <span class="highlight">love,
