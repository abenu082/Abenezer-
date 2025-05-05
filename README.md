# Abenezer-<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Abenezer Video Downloader</title>
  <!-- Font Awesome for icons -->
  <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: black;
      color: white;
      text-align: center;
      padding-top: 5rem;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
      text-shadow: 2px 2px 5px #333;
      font-family: serif;
    }

    input {
      padding: 15px 20px;
      font-size: 1rem;
      width: 300px;
      max-width: 90%;
      border: none;
      border-radius: 50px;
      outline: none;
      animation: floatInput 3s ease-in-out infinite;
    }

    @keyframes floatInput {
      0% { transform: translateY(0); }
      50% { transform: translateY(-8px); }
      100% { transform: translateY(0); }
    }

    button {
      padding: 12px 30px;
      border-radius: 10px;
      font-size: 1.1rem;
      border: none;
      background-color: #00bcd4;
      color: black;
      cursor: pointer;
      margin-top: 1rem;
      font-family: 'Segoe UI', sans-serif;
      font-weight: bold;
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: #0097a7;
    }

    #result {
      margin-top: 2rem;
      font-size: 1.2rem;
      text-shadow: 1px 1px 3px #000;
    }

    footer {
      margin-top: 4rem;
      font-size: 1rem;
      color: #ccc;
      padding-bottom: 2rem;
    }

    footer p {
      margin: 0.3rem 0;
    }

    /* Social Icons */
    .social-icons {
      position: fixed;
      top: 50%;
      left: 10px;
      transform: translateY(-50%);
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .social-icons a {
      color: white;
      font-size: 1.5rem;
      transition: transform 0.3s, color 0.3s;
    }

    .social-icons a:hover {
      color: #00bcd4;
      transform: scale(1.2);
    }
  </style>
</head>
<body>

  <h1>𝔞𝔟𝔢𝔫𝔢𝔷𝔢𝔯 𝔳𝔦𝔡𝔢𝔬 𝔡𝔬𝔴𝔫𝔩𝔬𝔞𝔡𝔢𝔯</h1>
  <p>Enter a video link below:</p>

  <input type="text" id="videoUrl" placeholder="Enter video URL..." />
  <br>
  <button onclick="downloadVideo()">𝑑𝑜𝑤𝑛𝑙𝑜𝑎𝑑</button>

  <div id="result"></div>

  <footer>
    <p>Contact me with email: <strong>Tabenezer02@gmail.com</strong></p>
    <p>Follow us on social media:</p>
    <p>Instagram: <strong>@Abe_nu082</strong></p>
    <p>TikTok: <strong>@butajiraweb</strong></p>
    <p>Telegram: <strong>@saver bot</strong></p>
  </footer>

  <!-- Floating Social Media Icons -->
  <div class="social-icons">
    <a href="https://instagram.com/Abe_nu082" target="_blank"><i class="fab fa-instagram"></i></a>
    <a href="https://www.tiktok.com/@butajiraweb" target="_blank"><i class="fab fa-tiktok"></i></a>
    <a href="https://youtube.com" target="_blank"><i class="fab fa-youtube"></i></a>
    <a href="https://t.me/saverbot" target="_blank"><i class="fab fa-telegram-plane"></i></a>
    <a href="https://facebook.com" target="_blank"><i class="fab fa-facebook"></i></a>
  </div>

  <script>
    function downloadVideo() {
      const url = document.getElementById('videoUrl').value;
      const result = document.getElementById('result');

      if (!url) {
        alert('Please enter a URL.');
        return;
      }

      result.innerHTML = "Downloading from: <br><strong>" + url + "</strong>";

      setTimeout(() => {
        result.innerHTML += "<br><br>Download complete!";
      }, 3000);
    }
  </script>

</body>
</html>
