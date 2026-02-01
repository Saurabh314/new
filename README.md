<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Be My Valentine 💖</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
  font-family: Arial, sans-serif;
  background: linear-gradient(135deg, #ff4d6d, #ff758f);
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0;
  color: white;
  text-align: center;
  overflow: hidden;
}

.card {
  background: rgba(0,0,0,0.2);
  padding: 30px;
  border-radius: 20px;
  max-width: 320px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.3);
}

h1 {
  font-size: 26px;
  margin-bottom: 10px;
}

p {
  font-size: 16px;
  margin-bottom: 25px;
}

button {
  font-size: 16px;
  padding: 10px 20px;
  border: none;
  border-radius: 30px;
  cursor: pointer;
  margin: 10px;
}

#yes {
  background: #2ecc71;
  color: white;
}

#no {
  background: #e74c3c;
  color: white;
  position: absolute;
}
</style>
</head>

<body>

<div class="card">
  <h1>Hey Chikku 🏐🏸🗣️🖋️❤️</h1>
  <p>
    From my heart to this screen…<br>
    Will you be my Valentine? 🌹
  </p>

  <button id="yes" onclick="sayYes()">Thik Chu 😻</button>
  <button id="no" onmouseover="moveNo()" ontouchstart="moveNo()">No 😅</button>
</div>

<script>
function sayYes() {
  document.body.innerHTML = `
  <div style="
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    flex-direction:column;
    background:linear-gradient(135deg,#ff4d6d,#ff758f);
    color:white;
    font-family:Arial;
    text-align:center;
    padding:20px;
  ">
    <h1>YAYYYY 💘🎉</h1>

    <p style="margin-bottom:20px;">
      दिल का दरिया बह ही गया 🥹❤️
    </p>

    <!-- PINTEREST IMAGE (DIRECT LINK) -->
    <img 
      src="https://i.pinimg.com/736x/14/d3/fb/14d3fbda2e8435231aeec66cddf7a6d3.jpg"
      style="
        width:260px;
        border-radius:20px;
        box-shadow:0 10px 25px rgba(0,0,0,0.4);
      "
    >
  </div>
  `;
}

function moveNo() {
  const button = document.getElementById("no");
  const x = Math.random() * (window.innerWidth - 120);
  const y = Math.random() * (window.innerHeight - 60);
  button.style.left = x + "px";
  button.style.top = y + "px";
}
</script>

</body>
</html>
