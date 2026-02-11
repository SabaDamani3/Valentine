<!DOCTYPE html>
<html>
<head>
  <title>Be My Valentine?</title>
  <style>
    body {
      text-align: center;
      font-family: Arial, sans-serif;
      background-color: #ffe6f0;
      margin-top: 100px;
    }
    h1 {
      font-size: 40px;
      color: #ff3366;
    }
    button {
      padding: 15px 25px;
      font-size: 18px;
      margin: 20px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      position: absolute;
    }
    #yes {
      background-color: #ff4d88;
      color: white;
      position: static;
    }
    #no {
      background-color: #999;
      color: white;
    }
  </style>
</head>
<body>

<h1>Will you be my Valentine? ❤️</h1>

<button id="yes" onclick="sayYes()">Yes 💕</button>
<button id="no">No 😢</button>

<script>
  const noBtn = document.getElementById("no");

  noBtn.addEventListener("mouseover", function() {
    const x = Math.random() * window.innerWidth * 0.8;
    const y = Math.random() * window.innerHeight * 0.8;
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
  });

  function sayYes() {
    document.body.innerHTML = "<h1>Yayyyyy!! 💖 I knew you'd say YES! 💍✨</h1>";
  }
</script>

</body>
</html>
