<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Video di Tengah</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.5.1/dist/confetti.browser.min.js"></script>
  <style>
    body {
      margin: 0;
      padding: 0;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4, #fbc2eb, #a6c1ee, #d4fc79, #96e6a1);
      background-size: 600% 600%;
      animation: gradientBG 20s ease infinite;
      font-family: 'Poppins', sans-serif;
      overflow-x: hidden;
    }

    @keyframes gradientBG {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    body::before {
      content: '';
      position: absolute;
      width: 100%;
      height: 100%;
      background-image: url('https://www.transparenttextures.com/patterns/cubes.png'),
                        url('https://www.transparenttextures.com/patterns/argyle.png');
      background-repeat: repeat;
      opacity: 0.1;
      z-index: 0;
    }

    h1 {
      color: white;
      font-size: 2.5rem;
      margin: 20px 0;
      font-weight: 600;
      z-index: 1;
    }

    .video-container {
      background: white;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
      padding: 20px;
      width: 60vw;
      max-height: 90vh;
      z-index: 1;
    }

    video {
      width: 100%;
      height: auto;
      border-radius: 10px;
    }

    .music-button {
      margin: 20px 0;
      padding: 10px 20px;
      font-size: 1rem;
      border: none;
      border-radius: 10px;
      background-color: #ffb6b9;
      color: white;
      cursor: pointer;
      transition: background-color 0.3s;
      font-family: 'Poppins', sans-serif;
      z-index: 1;
    }

    .music-button:hover {
      background-color: #ff6f91;
    }

    .photo-gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center; /* agar seperti chat bubble berjajar kiri */
      gap: 50px 60px; /* vertikal 50px, horizontal 60px */
      margin-bottom: 20px;
      padding: 20px;
      max-width: 90vw;
      z-index: 1;
    }

    .photo-item {
      position: relative;
      display: flex;
      flex-direction: column;
      align-items: center; /* bubble chat menempel kiri */
      width: 250px;
    }

    .photo-item img {
      width: 250px;
      height: 250px;
      object-fit: cover;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    }

    .photo-caption {
      margin-top: 8px;
      background: #ffffff;
      color: #333;
      padding: 10px 15px;
      border-radius: 20px 20px 20px 5px; /* bubble chat style */
      font-size: 0.9rem;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      white-space: nowrap;
      max-width: 240px;
      word-wrap: break-word;
    }
  </style>
</head>
<body>
  <h1>Enjoy Your New Journey!!</h1>
  <div class="video-container">
    <video controls>
      <source src="video.mp4" type="video/mp4">
      Browsermu tidak mendukung tag video.
    </video>
  </div>
  <button class="music-button" onclick="toggleMusic()">Play Music 🎵</button>

  <div class="photo-gallery">
    <div class="photo-item">
      <img src="photo1.png" alt="Photo 1">
      <div class="photo-caption">LDK NIH BOS😁</div>
    </div>
    <div class="photo-item">
      <img src="photo2.jpg" alt="Photo 2">
      <div class="photo-caption">Yalili mode versi ber 5</div>
    </div>
    <div class="photo-item">
      <img src="photo3.png" alt="Photo 3">
      <div class="photo-caption">seru bgt, sampe pengen nonjok</div>
    </div>
    <div class="photo-item">
      <img src="photo4.jpg" alt="Photo 4">
      <div class="photo-caption">canggung + polos😆</div>
    </div>
    <div class="photo-item">
        <img src="photo5.jpg" alt="Photo 4">
        <div class="photo-caption">ciailah after dauroh😋</div>
    </div>
    <div class="photo-item">
        <img src="photo6.jpg" alt="Photo 4">
        <div class="photo-caption">udah ga canggung nich😆</div>
    </div>
    <div class="photo-item">
        <img src="photo7.jpg" alt="Photo 4">
        <div class="photo-caption">HORE SPARVAL🧟</div>
    </div>
    <div class="photo-item">
        <img src="photo8.jpg" alt="Photo 4">
        <div class="photo-caption">mencari sponsor, berujung?</div>
    </div>
    <div class="photo-item">
        <img src="photo9.jpg" alt="Photo 4">
        <div class="photo-caption">kak nilna sakit</div>
    </div>
    <div class="photo-item">
        <img src="photo10.jpg" alt="Photo 4">
        <div class="photo-caption">bocah petualang</div>
    </div>
    <div class="photo-item">
        <img src="photo11.jpeg" alt="Photo 4">
        <div class="photo-caption">hah? ada apatuh!</div>
    </div>
    <div class="photo-item">
        <img src="photo12.jpeg" alt="Photo 4">
        <div class="photo-caption">allhamdulillah lengser</div>
    </div>
    <div class="photo-item">
        <img src="photo13.jpg" alt="Photo 4">
        <div class="photo-caption">ka nilna marah fotonya cmn ber4</div>
    </div>
    <div class="photo-item">
        <img src="photo14.jpeg" alt="Photo 4">
        <div class="photo-caption">semakin bahagia</div>
    </div>
    <div class="photo-item">
        <img src="photo15.jpeg" alt="Photo 4">
        <div class="photo-caption">pose andalan bos</div>
    </div>
    <div class="photo-item">
        <img src="photo16.jpeg" alt="Photo 4">
        <div class="photo-caption">KUAT! KUAT!KUAT</div>
      </div>
  </div>

  <audio id="bg-music" loop>
    <source src="butterflies.mp3" type="audio/mp3">
    Browsermu tidak mendukung tag audio.
  </audio>

  <script>
    const music = document.getElementById('bg-music');
    const button = document.querySelector('.music-button');

    function toggleMusic() {
      if (music.paused) {
        music.play();
        button.textContent = 'Pause Music ⏸️';
      } else {
        music.pause();
        button.textContent = 'Play Music 🎵';
      }
    }

    // Trigger confetti when page loads
    window.onload = () => {
      confetti({
        particleCount: 200,
        spread: 100,
        origin: { y: 0.6 },
      });
    };
  </script>
</body>
</html>
