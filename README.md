<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Personal Website</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body, html {
      height: 100%;
      overflow: hidden;
      background-color: #141E30;
      color: white;
      font-size: 1.3rem;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    .enter-screen {
      background: linear-gradient(135deg, #141E30, #243B55);
      color: white;
      height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      transition: opacity 0.8s ease;
      padding: 20px;
      text-align: center;
    }

    .enter-screen button {
      padding: 14px 28px;
      font-size: 1.5rem;
      background-color: #ffffff;
      color: #141E30;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      margin-top: 20px;
      transition: background 0.3s, color 0.3s;
    }

    .enter-screen button:hover {
      background-color: #ddd;
      color: #000;
    }

    .main-content {
      display: none;
      padding: 60px 80px;
      height: 100vh;
      overflow-y: auto;
      background-color: #1f2a38;
    }

    .main-content p {
      margin-bottom: 1.5rem;
      line-height: 1.8;
    }
  </style>
</head>
<body>

  <div class="enter-screen" id="enterScreen">
    <h1>Welcome to My Website</h1>
    <button onclick="enterSite()">Enter</button>
  </div>

  <div class="main-content" id="mainContent">
    <h1>Hi, I'm Narayana</h1>
    <p>About me:</p>
    <p>Iam doing my bachelors in Loyola ICAM College Of Engineering and Technology.</p>
    <p>Iam interested in python programming. I wish to become an Enterpreneur.</p>
    <p>I also wish to work abroad.</p>
    <p>Email:<a href="https://mail.google.com/mail/?view=cm&fs=1&to=deva02072007@gmail.com" target="_blank">deva02072007@gmail.com</a>
    <p>Phone: 8610312853</p>
</div>

  <script>
    function enterSite() {
      const enterScreen = document.getElementById('enterScreen');
      const mainContent = document.getElementById('mainContent');

      enterScreen.style.opacity = '0';
      setTimeout(() => {
        enterScreen.style.display = 'none';
        mainContent.style.display = 'block';
      }, 800);
    }
  </script>

</body>
</html>

