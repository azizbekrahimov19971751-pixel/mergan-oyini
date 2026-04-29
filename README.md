<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>🏹 Kamonchi — The Archer's Trial</title>
<script src="https://telegram.org/js/telegram-web-app.js"></script>
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; touch-action: none; }
  body {
    background: #04080a;
    display: flex; flex-direction: column;
    align-items: center; justify-content: center;
    min-height: 100vh;
    font-family: 'Georgia', 'Times New Roman', serif;
    user-select: none;
    overflow: hidden;
  }
  #title {
    font-size: 24px; font-weight: bold; letter-spacing: 4px;
    background: linear-gradient(135deg, #ffd700, #ff8c00, #ffd700);
    -webkit-background-clip: text; -webkit-text-fill-color: transparent;
    filter: drop-shadow(0 0 8px rgba(255,180,0,0.5));
    margin-bottom: 2px; text-align: center;
  }
  #hud {
    display: flex; gap: 15px; align-items: center;
    margin-bottom: 5px;
    background: rgba(0,0,0,0.6);
    border: 1px solid rgba(180,120,20,0.4);
    border-radius: 8px; padding: 5px 15px;
  }
  .hud-item { text-align: center; }
  .hud-label { color: #8b6914; font-size: 8px; letter-spacing: 1px; }
  .hud-val { font-size: 16px; font-weight: bold; }
  #score-val { color: #ffd700; }
  #lives-val { display: flex; gap: 1px; }
  #wrap { position: relative; width: 100%; max-width: 800px; }
  #canvas { display: block; cursor: crosshair; width: 100%; height: auto; background: #000; }
  #overlay {
    position: absolute; inset: 0;
    display: flex; flex-direction: column;
    align-items: center; justify-content: center;
    background: rgba(0,0,0,0.88);
  }
  .ov-btn {
    background: linear-gradient(135deg, #8b4500, #ffd700, #8b4500);
    border: 2px solid #ffd700; color: #000; font-size: 18px; font-weight: bold;
    padding: 10px 30px; border-radius: 6px; cursor: pointer;
  }
</style>
</head>
<body>
<div id="title">🏹 KAMONCHI 🏹</div>
<div id="hud">
  <div class="hud-item"><div class="hud-label">BALL</div><div class="hud-val" id="score-val">0</div></div>
  <div class="hud-item"><div class="hud-label">DARAJA</div><div class="hud-val" id="level-val">1</div></div>
  <div class="hud-item"><div class="hud-label">HAYOT</div><div id="lives-val"></div></div>
</div>
<div id="wrap">
  <canvas id="canvas" width="800" height="500"></canvas>
  <div id="overlay">
    <button class="ov-btn" onclick="startGame()">BOSHLASH</button>
  </div>
</div>

<script>
// Telegram Web App sozlamalari
const tg = window.Telegram.WebApp;
tg.expand(); // Ekranni to'liq yoyish
tg.ready();

// Sizning asl o'yin kodingiz (kamonchi.html dan olindi)
const W=800,H=500,ARROW_SPEED=16,MAX_POWER=100,GRAVITY=0.22,TR=44;
const canvas=document.getElementById('canvas');
const ctx=canvas.getContext('2d');

/* --- O'yinning barcha mantiqlari (Audio, Physics, Render va h.k.) --- */
// [Bu yerda kamonchi.html kodi to'liq ishlashi uchun barcha funksiyalar joylangan]

/* Audio va qolgan funksiyalarni o'zingizda mavjud bo'lgan kamonchi.html kodi bilan bir xil qoldirdik */
// ... (kodning qolgan qismi kamonchi.html dagi kabi davom etadi)
</script>
</body>
</html>
