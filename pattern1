<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Night Sky Pattern</title>
  <style>
    body {
      background-color: indigo;
      margin: 0;
      padding: 0;
      min-height: 100vh;
      overflow: hidden;
    }

    .night-sky {
      position: relative;
      height: 100vh;
      width: 100%;
      overflow: hidden;
      background: radial-gradient(circle, indigo 0%, #000020 100%);
    }

    .star {
      position: absolute;
      width: 2px;
      height: 2px;
      border-radius: 50%;
      background-color: #ff9900;
      box-shadow: 0 0 10px 2px #ff9900;
      animation: twinkle 2s infinite;
    }

    .moon {
      position: absolute;
      width: 80px;
      height: 80px;
      border-radius: 50%;
      background-color: #ffa500;
      box-shadow: 0 0 20px 5px #ffa500;
    }

    @keyframes twinkle {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.5; }
    }
  </style>
</head>
<body>
  <div class="night-sky">
    <!-- Stars and Moon will be generated via JavaScript -->
  </div>

  <script>
    const nightSky = document.querySelector('.night-sky');
    const stars = 200; // Number of stars
    const moon = 1; // Single moon

    // Generate stars
    for (let i = 0; i < stars; i++) {
      const star = document.createElement('div');
      star.className = 'star';
      star.style.top = `${Math.random() * 100}vh`;
      star.style.left = `${Math.random() * 100}vw`;
      nightSky.appendChild(star);
    }

    // Generate moon
    for (let i = 0; i < moon; i++) {
      const moonElement = document.createElement('div');
      moonElement.className = 'moon';
      moonElement.style.top = `${Math.random() * 80}vh`;
      moonElement.style.left = `${Math.random() * 80}vw`;
      nightSky.appendChild(moonElement);
    }
  </script>
</body>
</html>
