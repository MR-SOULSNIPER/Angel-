<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For My Valentine ❤️</title>

<style>
body {
  margin: 0;
  font-family: 'Comic Sans MS', cursive;
  background: linear-gradient(#ffb6c1, #ffe4e1);
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.page {
  display: none;
  text-align: center;
}

.page.active {
  display: block;
}

.paper {
  background: white;
  padding: 25px;
  width: 280px;
  border-radius: 12px;
  box-shadow: 0 8px 15px rgba(0,0,0,0.25);
  margin: auto;
}

.paper h1 {
  color: #e75480;
  font-size: 22px;
}

.paper p {
  color: #444;
  font-size: 16px;
  line-height: 1.5;
}

.bear {
  font-size: 150px;
  margin-top: 10px;
}

button {
  margin-top: 15px;
  padding: 10px 18px;
  border: none;
  border-radius: 20px;
  background: #ff69b4;
  color: white;
  font-size: 14px;
  cursor: pointer;
}

button:hover {
  background: #ff1493;
}
</style>
</head>

<body>

<!-- PAGE 1 -->
<div class="page active">
  <div class="paper">
    <h1>Hey My Love ❤️</h1>
    <p>
      I made this just for you.<br>
      Every word here comes from my heart.<br>
      Please keep going.
    </p>
    <button onclick="nextPage()">Next</button>
  </div>
  <div class="bear">🧸</div>
</div>

<!-- PAGE 2 -->
<div class="page">
  <div class="paper">
    <p>
      You mean more to me than I’ve ever been able to explain.<br><br>
      You aren’t just someone I love —  
      you’re someone who changed me for the better.
    </p>
    <button onclick="nextPage()">Next</button>
  </div>
  <div class="bear">🧸</div>
</div>

<!-- PAGE 3 -->
<div class="page">
  <div class="paper">
    <p>
      When I think about my happiest moments,<br>
      you’re always there.<br><br>
      Your smile, your voice, the way you make everything feel lighter —
      it all lives in my heart.
    </p>
    <button onclick="nextPage()">Next</button>
  </div>
  <div class="bear">🧸</div>
</div>

<!-- PAGE 4 -->
<div class="page">
  <div class="paper">
    <p>
      You make me feel safe.<br>
      You make me feel loved.<br>
      You make me feel like I’m finally home.<br><br>
      I’m grateful for you every single day.
    </p>
    <button onclick="nextPage()">Next</button>
  </div>
  <div class="bear">🧸</div>
</div>

<!-- PAGE 5 -->
<div class="page">
  <div class="paper">
    <h1>My Valentine 💖</h1>
    <p>
      I promise to choose you.<br>
      To care for you.<br>
      To love you in the good days and the hard ones.<br><br>
      Forever isn’t long enough with you.
    </p>
  </div>
  <div class="bear">🧸❤️</div>
</div>

<script>
let currentPage = 0;
const pages = document.querySelectorAll('.page');

function nextPage() {
  pages[currentPage].classList.remove('active');
  currentPage++;
  pages[currentPage].classList.add('active');
}
</script>

</body>
</html>
