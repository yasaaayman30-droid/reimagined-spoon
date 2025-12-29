<!DOCTYPE html><html lang="ar">
<head>
  <meta charset="UTF-8" />
  <title>عيد ميلاد مجيد يا ميرنا</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(135deg, #b30000, #006400);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Arial', sans-serif;
      overflow: hidden;
      color: #fff;
      text-align: center;
    }.card {
  background: rgba(0,0,0,0.4);
  padding: 40px;
  border-radius: 25px;
  box-shadow: 0 0 30px rgba(255,255,255,0.3);
  animation: pop 1.5s ease;
}

h1 {
  font-size: 32px;
  margin-bottom: 15px;
}

h2 {
  font-size: 26px;
  color: #ffcccc;
}

.icons {
  font-size: 45px;
  margin-top: 20px;
  animation: float 3s infinite ease-in-out;
}

.heart {
  position: absolute;
  color: pink;
  font-size: 24px;
  animation: hearts 5s linear infinite;
}

@keyframes float {
  0% { transform: translateY(0); }
  50% { transform: translateY(-15px); }
  100% { transform: translateY(0); }
}

@keyframes pop {
  from { transform: scale(0.5); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}

@keyframes hearts {
  0% { bottom: -10%; opacity: 0; }
  20% { opacity: 1; }
  100% { bottom: 110%; opacity: 0; }
}

  </style>
</head>
<body>  <div class="card">
    <h1>🎉 كل سنة وانتي طيبة 🎉</h1>
    <h2>عيد ميلاد مجيد<br>أحلى ميرنا 💖</h2>
    <div class="icons">🎅 🎄 🎁</div>
  </div>  <!-- قلوب متحركة -->  <script>
    function createHeart() {
      const heart = document.createElement('div');
      heart.className = 'heart';
      heart.innerHTML = '❤';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = (3 + Math.random() * 3) + 's';
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }

    setInterval(createHeart, 500);
  </script></body>
</html># reimagined-spoon
