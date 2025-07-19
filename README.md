<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Defaced by Junin Labaxuria</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Orbitron&display=swap');

    body {
      margin: 0;
      padding: 0;
      background: radial-gradient(circle at center, #8B0000, #000000);
      color: #FF0000;
      font-family: 'Orbitron', sans-serif;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
    }

    .container {
      text-align: center;
      animation: flicker 3s infinite;
    }

    h1 {
      font-size: 6rem;
      margin: 0 0 1rem 0;
      text-shadow: 0 0 10px #FF0000, 0 0 20px #FF4500;
    }

    p {
      font-size: 2rem;
      letter-spacing: 0.1em;
      text-shadow: 0 0 5px #FF6347;
    }

    .instagram-link {
      color: #FF4500;
      font-weight: bold;
      text-decoration: none;
      font-size: 2rem;
      margin-top: 1rem;
      display: inline-block;
      text-shadow: 0 0 5px #FF6347;
    }

    button {
      margin-top: 2rem;
      padding: 1rem 2rem;
      font-size: 1.5rem;
      font-weight: bold;
      color: #fff;
      background-color: #8B0000;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      text-shadow: 0 0 5px #FF4500;
    }

    button:hover {
      background-color: #FF4500;
    }

    iframe#ytplayer {
      width: 1px;
      height: 1px;
      border: none;
      visibility: hidden;
    }

    @keyframes flicker {
      0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% { opacity: 1; }
      20%, 22%, 24%, 55% { opacity: 0.4; }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>HACKED</h1>
    <p>Defacement por Junin Labaxuria</p>
    <p>Este site foi invadido</p>
    <a href="https://www.instagram.com/junin_labaxurias?igsh=MWoyMHB1b3hxcmJqZw==" class="instagram-link" target="_blank">@junin_labaxurias</a>
    <button id="playMusic">▶️ Tocar Música</button>
    <iframe id="ytplayer" src="https://www.youtube.com/embed/ah5W_O4neU4?enablejsapi=1&autoplay=1" allow="autoplay"></iframe>
  </div>

  <script>
    document.getElementById('playMusic').addEventListener('click', () => {
      const iframe = document.getElementById('ytplayer');
      iframe.style.visibility = 'visible';
      // Envia comando de play
      iframe.contentWindow.postMessage('{"event":"command","func":"playVideo","args":""}', '*');
      document.getElementById('playMusic').style.display = 'none';
    });
  </script>
</body>
</html>
