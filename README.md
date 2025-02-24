<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&display=swap" rel="stylesheet">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday</title>
  <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css" />
  <style>
    body {
      margin: 0;
      background-color: #450000;
      overflow-x: hidden; /* Disable horizontal scrolling */
      font-family: 'Playfair Display', serif;
    }

    .password-container {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #450000;
      color: white;
      z-index: 10;
      position: fixed;
      width: 100%;
      top: 0;
      left: 0;
    }

    .password-box {
      background-color: rgba(255, 255, 255, 0.1);
      padding: 40px;
      border-radius: 15px;
      text-align: center;
      max-width: 500px;
      width: 80%;
    }

    .password-title {
      font-size: 32px;
      margin-bottom: 20px;
    }

    .password-input {
      width: 100%;
      padding: 15px;
      margin: 20px 0;
      border: none;
      border-radius: 5px;
      font-size: 18px;
      background-color: rgba(255, 255, 255, 0.9);
    }

    .password-button {
      background-color: white;
      color: #450000;
      border: none;
      padding: 15px 30px;
      border-radius: 5px;
      font-size: 18px;
      cursor: pointer;
      transition: all 0.3s;
    }

    .password-button:hover {
      background-color: #e0e0e0;
    }

    .password-hint {
      margin-top: 20px;
      font-size: 16px;
      opacity: 0;
      transition: opacity 0.5s;
    }

    .hidden {
      display: none;
    }

    .birthday-text {
      font-family: 'Playfair Display', serif;
      font-size: 100px;
      margin-top: 100px;
      text-align: center;
      color: #ffffff;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
      position: relative;
      font-weight: 700;
      z-index: 3;
    }

    .video-container {
      position: relative;
      width: 100%;
      max-width: 1000px;
      margin: 50px auto;
      padding-top: 25%; 
    }

    .video-container iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      border: none;
    }

    .message-container {
      font-family: 'Playfair Display', serif;
      color: #000000;
      text-align: center;
      padding: 40px;
      margin: 50px auto;
      max-width: 800px;
      position: relative;
      z-index: 3;
      background-color: white;
      border-radius: 15px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    .name {
      font-size: 50px;
      margin-bottom: 10px;
    }

    .quote {
      font-size: 36px;
      font-weight: 800;
      margin-bottom: 20px;
    }

    .message {
      font-size: 20px;
      line-height: 1.6;
      white-space: pre-line;
    }

    .swiper-container {
      width: 80%;
      height: auto;
      margin: 50px auto;
      position: relative;
    }

    .swiper-slide img {
      width: auto;
      height: calc(100vw * 9 / 16); 
      display: block;
      margin: 0 auto;
      border-radius: 15px;
    }

    .swiper-slide iframe {
      width: 100%; 
      max-width: 800px; 
      height: 800px; 
      display: block;
      margin: 0 auto;
      border-radius: 15px;
    }

    .swiper-button-next,
    .swiper-button-prev {
      top: 50%;
      transform: translateY(-50%);
    }

    .content-container {
      display: none;
    }
  </style>
</head>
<body>
  <!-- Password Gate -->
  <div id="passwordContainer" class="password-container">
    <div class="password-box">
      <div class="password-title">Enter Password</div>
      <input type="password" id="passwordInput" class="password-input" placeholder="Password">
      <button id="submitButton" class="password-button">Enter</button>
      <div id="passwordHint" class="password-hint">Hint: When we first met (format: DDMMYYYY)</div>
    </div>
  </div>

  <div id="contentContainer" class="content-container">
    <div class="container">
      <div class="birthday-text">Happy Birthday Praditya!</div>
      <div class="video-container">
        <iframe 
          src="3.mp4" 
          title="Birthday Video" 
          allow="autoplay; encrypted-media" 
          allowfullscreen>
        </iframe>
      </div>
      <div class="message-container">
        <div class="name">Praditya Putra Irawan</div>
        <div class="quote">Until Every Last Star In The Galaxy Dies</div>
        <div class="message">
          Happy birthday Pradityaaa!! Congratulations on successfully making it through another year^_^ Kalau ditanya kenapa manggil praditya, aku mau beda. Aku mau selalu beda di mata kamu. Dalam hal apapun itu. You deserve every good thing that comes your way. May every new chapter be better than your last. Kalau di Tarot - .feast "Kutanggung denganmu Selama ku mampu" i will do that to you Praditya. Setelah apa aja yang udah kita laluin "Namun Padamu ku percaya Tak masuk logika". Memang tidak akan pernah masuk logika kenapa bisa sepercaya ini. Did you know that you play in my mind like one of my favorite song lyrics? Understand-Keshi "You're the only one who understands". Yap, kamu yang paling ngerti semuanya Praditya. And always you. Untuk terakhir kalinya, I hope your day is everything you want it to be. In Islam say "Barakallah Fii Umrik" but in kristen we say "Proverbs 3:16 Long life in his right hand; in his left hand are riches and honor" Enjoy your twenty!!
        </div>
      </div>
      <div class="swiper-container">
        <div class="swiper-wrapper">
          <div class="swiper-slide"><img src="1.png" alt="Foto 1"></div>
          <div class="swiper-slide"><img src="2.jpg" alt="Foto 2"></div>
          <div class="swiper-slide"><img src="3.jpg" alt="Foto 3"></div>
          <div class="swiper-slide"><img src="4.jpg" alt="Foto 4"></div>
          <div class="swiper-slide"><img src="5.jpg" alt="Foto 5"></div>
          <div class="swiper-slide"><img src="6.jpg" alt="Foto 6"></div>
          <div class="swiper-slide"><img src="7.jpg" alt="Foto 7"></div>
          <div class="swiper-slide"> 
            <iframe 
              src="8.mp4" 
              title="Birthday Video" 
              allow="autoplay; encrypted-media" 
              allowfullscreen>
            </iframe>
          </div>
        </div>
        <div class="swiper-button-next"></div>
        <div class="swiper-button-prev"></div>
        <div class="swiper-pagination"></div>
      </div>
    </div>
  </div>

  <script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>
  <script>
    let attempts = 0;
    const correctPassword = "10082024";
    const passwordInput = document.getElementById("passwordInput");
    const submitButton = document.getElementById("submitButton");
    const passwordContainer = document.getElementById("passwordContainer");
    const contentContainer = document.getElementById("contentContainer");
    const passwordHint = document.getElementById("passwordHint");

    submitButton.addEventListener("click", checkPassword);
    passwordInput.addEventListener("keypress", function(event) {
      if (event.key === "Enter") {
        checkPassword();
      }
    });

    function checkPassword() {
      const enteredPassword = passwordInput.value;
      
      if (enteredPassword === correctPassword) {
        passwordContainer.style.display = "none";
        contentContainer.style.display = "block";
        const swiper = new Swiper('.swiper-container', {
          loop: true,
          pagination: {
            el: '.swiper-pagination',
            clickable: true,
          },
          navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev',
          },
        });
      } else {
        attempts++;
        passwordInput.value = "";
        passwordInput.placeholder = "Incorrect password";
        
        if (attempts >= 1) {
          passwordHint.style.opacity = "1";
        }
        passwordInput.classList.add("shake");
        setTimeout(() => {
          passwordInput.classList.remove("shake");
        }, 500);
      }
    }
  </script>
</body>
</html>
