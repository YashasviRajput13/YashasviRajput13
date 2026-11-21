<div class="game">
  <div class="dino">🦖</div>
  <div class="cactus">🌵</div>
</div>

<style>
.game {
  position: relative;
  width: 100%;
  height: 120px;
  overflow: hidden;
  background: #0d1117;
  border-bottom: 2px dashed #888;
}

.dino {
  position: absolute;
  left: 70px;
  bottom: 0;
  font-size: 40px;
  transform: scaleX(-1);
  z-index: 2;
}

.cactus {
  position: absolute;
  bottom: 0;
  left: 100%;
  font-size: 30px;
  animation: cactusMove 2.8s linear infinite;
}

@keyframes cactusMove {
  from { left: 100%; }
  to { left: -40px; }
}

.dino.jump {
  animation: dinoJump 850ms ease-in-out;
}

@keyframes dinoJump {
  0%   { bottom: 0; }
  40%  { bottom: 75px; }
  60%  { bottom: 75px; }
  100% { bottom: 0; }
}
</style>

<script>
const dino = document.querySelector(".dino");
const cactus = document.querySelector(".cactus");

let jumping = false;
let jumpedForThisCactus = false;

function gameLoop() {
  const dinoRect = dino.getBoundingClientRect();
  const cactusRect = cactus.getBoundingClientRect();

  const distance = cactusRect.left - dinoRect.right;

  // Jump when cactus is very close
  if (
    distance > 0 &&
    distance < 45 &&
    !jumping &&
    !jumpedForThisCactus
  ) {
    jumping = true;
    jumpedForThisCactus = true;

    dino.classList.add("jump");

    setTimeout(() => {
      dino.classList.remove("jump");
      jumping = false;
    }, 850);
  }

  // Reset after cactus passes
  if (cactusRect.right < dinoRect.left) {
    jumpedForThisCactus = false;
  }

  requestAnimationFrame(gameLoop);
}

gameLoop();
</script>


---

<h1 align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Caveat&weight=700&size=45&duration=1&pause=999999&color=FF4F81&center=true&vCenter=true&width=650&lines=Hello!+I'm+Yashasvi+Singh+Rajput" />
</h1>

---

## 💡 What do I know?

- 🚀 Full Stack Development (React + Java Backend)  
- 🤖 AI/ML Development & Intelligent Systems  
- 🧠 Strong in DSA, OOP, DBMS, OS, Computer Networks  
- 🏆 Hackathon Builder & Competitive Programmer  

---

## 💻 My Tech Stack

<div align="center">
<img src="Images/img1.png" width="100%" />
</div>

---

## 🎬 Dev Vibes

<div align="center">
<img src="Gifs/gif1.gif" width="220"/>
</div>

---

## 🧠 What I Focus On

- Backend Engineering (Java + Spring Boot)  
- Full Stack Development (React.js)  
- Database Systems (MySQL, MongoDB)  
- AI/ML + Automation  

---

## ⚡ Fun Facts / Hobbies

- 🏊 Swimming  
- 📖 Enjoy reading fiction  
- ♟️ Playing chess  
- 🧠 Solving Rubik's Cube  

---

## 🌐 Where to find me

<p>
<a href="https://twitter.com/YashasviRajput13"><img src="https://img.shields.io/badge/twitter-%231DA1F2.svg?style=for-the-badge&logo=twitter&logoColor=white"/></a>
<a href="https://www.linkedin.com/in/yashasvi-s-rajput-492154319"><img src="https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="https://github.com/YashasviRajput13"><img src="https://img.shields.io/badge/github-%23000000.svg?style=for-the-badge&logo=github&logoColor=white"/></a>
</p>

---

## 📌 Featured Work

<div align="center">
<img src="https://emoji.gg/assets/emoji/7524_this_animated_bottom.gif">
</div>

---

<div align="center">
<img src="https://github-readme-streak-stats.herokuapp.com/?user=YashasviRajput13&theme=radical"/>
</div>

---

<div align="center">
✨ Building scalable systems, not just writing code ✨
</div>
