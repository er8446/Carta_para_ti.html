<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Para Saray 💖</title>
  <style>
    body {
      background: black;
      color: white;
      text-align: center;
      font-family: 'Courier New', monospace;
      overflow: hidden;
    }

    .heart {
      position: absolute;
      animation: float 10s infinite;
      color: pink;
      font-size: 2em;
    }

    @keyframes float {
      0% { transform: translateY(100vh) scale(1); opacity: 1; }
      100% { transform: translateY(-100vh) scale(0.5); opacity: 0; }
    }
  </style>
</head>
<body>
  <h1>Te amo, Saray 💕</h1>
  <p>Esta carta es para recordarte lo mucho que te amo y todo lo que significas para mí.</p>

  <!-- Corazones flotando -->
  <script>
    setInterval(() => {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.innerText = "❤️";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = Math.random() * 2 + 1 + "em";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 10000);
    }, 300);
  </script>
</body>
</html>
