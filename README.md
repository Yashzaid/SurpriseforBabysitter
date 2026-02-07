<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>One Honest Question ❤️</title>

<style>
body {
  margin: 0;
  height: 100vh;
  background: linear-gradient(135deg, #ff9a9e, #fad0c4);
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'Arial', sans-serif;
}

.card {
  background: white;
  padding: 40px;
  border-radius: 22px;
  text-align: center;
  box-shadow: 0 25px 45px rgba(0,0,0,0.2);
  max-width: 440px;
}

h1, h2 {
  color: #ff4d6d;
}

p {
  font-size: 18px;
  color: #444;
  line-height: 1.5;
}

.buttons {
  margin-top: 30px;
  position: relative;
  height: 130px;
}

button {
  padding: 12px 36px;
  font-size: 16px;
  border: none;
  border-radius: 30px;
  cursor: pointer;
}

#yes {
  background: #ff4d6d;
  color: white;
  transition: transform 0.3s;
}

#yes:hover {
  transform: scale(1.15);
}

#no {
  background: #eee;
  color: #333;
  position: absolute;
  left: 160px;
  top: 60px;
}
</style>
</head>

<body>

<div class="card" id="card">
  <h1>Hey Babysitter ❤️</h1>

  <p>
    I’ve been thinking about this more than I’ll admit 😌<br><br>
    You make ordinary moments feel special.  
    You make me smile without even trying.  
    And somehow… you became my favorite person 💕<br><br>
    So here’s my very serious question…
  </p>

  <h2>
    Will you be my best friend,<br>
    my girlfriend,<br>
    my partner,<br>
    and someday… my future wife? ❤️
  </h2>

  <div class="buttons">
    <button id="yes" onclick="yesClicked()">YES 😍</button>
    <button id="no">NO 🙈</button>
  </div>
</div>

<script>
const noBtn = document.getElementById("no");

function moveNo() {
  const maxX = 260;
  const maxY = 110;

  const x = Math.random() * maxX;
  const y = Math.random() * maxY;

  noBtn.style.left = x + "px";
  noBtn.style.top = y + "px";
}

// Infinite movement (mobile + desktop)
setInterval(moveNo, 700);
noBtn.addEventListener("touchstart", moveNo);
noBtn.addEventListener("mouseover", moveNo);
noBtn.addEventListener("click", moveNo);

function yesClicked() {
  document.getElementById("card").innerHTML = `
    <h1>HAHA 😄❤️</h1>
    <p>
      Joking 😌<br><br>
      I just wanted to tease you and annoy you a little 😉<br><br>
      But honestly… you are really the best friend I’ve ever got,  
      and I’m truly glad to have you in my life.<br><br>
      I hope you stay with me forever ❤️
    </p>
    <div style="font-size:46px;">❤️ ❤️ ❤️ ❤️ ❤️</div>
  `;
}
</script>

</body>
</html>
