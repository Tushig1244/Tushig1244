<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Will You Be My Valentine?</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
      background-color: #fff;
      margin: 0;
      padding: 0;
    }
    h1 {
      color: #ff69b4;
      font-size: 2.5em;
      margin-top: 50px;
    }
    .buttons {
      margin-top: 20px;
    }
    .button {
      background-color: #ff69b4;
      color: white;
      border: none;
      padding: 10px 20px;
      margin: 5px;
      font-size: 1.2em;
      cursor: pointer;
      border-radius: 5px;
      transition: background-color 0.3s, transform 0.3s;
    }
    .button:hover {
      background-color: #ff1493;
      transform: scale(1.1);
    }
    .gif {
      margin-top: 30px;
      opacity: 0;
      transition: opacity 1s ease-in-out;
    }
    .gif.visible {
      opacity: 1;
    }
    p {
      font-size: 1.2em;
      color: #333;
    }
  </style>
</head>
<body>
  <h1>Will you be my valentine?</h1>
  <div class="buttons">
    <button class="button" onclick="showGif()">Yes</button>
    <button class="button" onclick="reject()">I do no wanna o(TヘTo)</button>
  </div>
  <div class="gif" id="gif">
    <img src="https://media.giphy.com/media/3o7abldj0b3rxrZUxW/giphy.gif" alt="Cat begging" width="300">
    <p>Pleeease</p>
  </div>
  <script>
    function showGif() {
      document.getElementById('gif').classList.add('visible');
    }

    function reject() {
      const button = document.querySelector('.buttons .button:nth-child(2)');
      button.textContent = "Are you suuuure? 😢";
      button.style.backgroundColor = "#ff6347";
    }
  </script>
</body>
</html>
