<div align="center">

<!-- Google Fonts for Poppins and a Retro Game Font -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;800&family=Press+Start+2P&display=swap" rel="stylesheet">

<style>
  /* 
    Note: Some Markdown renderers (like standard GitHub) might strip out <style> tags for security.
    However, this will look incredible in VSCode previews, custom websites, or MDX setups! 
  */
  .game-container {
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(135deg, #0f0f1b, #1a1a2e);
    color: #e0e0e0;
    padding: 40px;
    border: 4px solid #4a00e0;
    border-radius: 20px;
    box-shadow: 0 0 25px #8e2de2, inset 0 0 20px #4a00e0;
    position: relative;
    overflow: hidden;
    max-width: 850px;
    margin: 0 auto;
    text-align: center;
  }
  
  .game-header {
    font-family: 'Press Start 2P', cursive;
    color: #00ffcc;
    text-shadow: 3px 3px 0px #ff0055;
    animation: pulse 2s infinite;
    margin-bottom: 30px;
    font-size: 2.2em;
  }

  .quest-box {
    border: 4px dashed #ff0055;
    padding: 20px;
    margin: 25px 0;
    background: rgba(255, 0, 85, 0.1);
    border-radius: 12px;
    transition: all 0.3s ease;
    text-align: left;
  }

  .quest-box:hover {
    transform: scale(1.03);
    border-color: #00ffcc;
    background: rgba(0, 255, 204, 0.1);
    box-shadow: 0 0 15px rgba(0, 255, 204, 0.4);
  }

  .quest-title {
    font-family: 'Press Start 2P', cursive;
    font-size: 1.2em;
    color: #fff;
    margin-top: 0;
  }

  @keyframes pulse {
    0% { transform: scale(1); }
    50% { transform: scale(1.03); }
    100% { transform: scale(1); }
  }

  .btn-start {
    display: inline-block;
    padding: 15px 30px;
    font-family: 'Press Start 2P', cursive;
    font-size: 16px;
    color: #fff;
    background: linear-gradient(45deg, #ff0055, #8e2de2);
    border: 3px solid #fff;
    border-radius: 8px;
    text-decoration: none;
    cursor: pointer;
    box-shadow: 0 5px 20px rgba(255, 0, 85, 0.5);
    animation: float 3s ease-in-out infinite;
    transition: filter 0.3s ease;
  }

  .btn-start:hover {
    filter: brightness(1.2);
  }

  @keyframes float {
    0% { transform: translateY(0px); }
    50% { transform: translateY(-10px); }
    100% { transform: translateY(0px); }
  }

  .inventory-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 20px;
    margin-top: 30px;
  }

  .item-card {
    background: rgba(255, 255, 255, 0.05);
    border: 2px solid #00ffcc;
    border-radius: 12px;
    padding: 20px;
    text-align: center;
    box-shadow: 0 0 15px rgba(0, 255, 204, 0.15);
    transition: transform 0.2s ease;
  }

  .item-card:hover {
    transform: translateY(-5px);
    background: rgba(255, 255, 255, 0.1);
  }

  .item-value {
    font-family: 'Press Start 2P', cursive;
    font-size: 1.2em;
    color: #ff0055;
    margin-bottom: 10px;
  }

  .item-label {
    font-size: 0.9em;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 600;
    color: #b3b3b3;
  }
  
  .hp-bar-container {
    width: 100%;
    background: #333;
    border: 3px solid #fff;
    border-radius: 10px;
    height: 25px;
    margin-bottom: 20px;
    overflow: hidden;
  }
  
  .hp-bar-fill {
    height: 100%;
    background: linear-gradient(90deg, #ff0055, #ffcc00);
    width: 100%;
    animation: hp-drain 4s infinite alternate ease-in-out;
  }
  
  @keyframes hp-drain {
    0% { width: 100%; }
    100% { width: 85%; }
  }
</style>

<div class="game-container">
  
  <h1 class="game-header">▶ PLAYER 1 READY</h1>
  
  <div class="hp-bar-container">
    <div class="hp-bar-fill"></div>
  </div>
  
  <p style="font-size: 20px; line-height: 1.8; margin-bottom: 30px;">
    Welcome to my digital realm! 🚀 I'm a developer who crafts interactive experiences, levels up daily, and conquers bugs in the matrix.
  </p>

  <div class="quest-box">
    <h2 class="quest-title">⚔️ Current Quest</h2>
    <p style="font-size: 16px; line-height: 1.5; font-family: 'Poppins', sans-serif;">
      Exploring the outer limits of web development, building epic portfolios, and mastering the arcane arts of HTML, CSS, and JavaScript. 
    </p>
  </div>

  <div class="inventory-grid">
    <div class="item-card">
      <div class="item-value">LVL 99</div>
      <div class="item-label">Frontend</div>
    </div>
    <div class="item-card">
      <div class="item-value">100%</div>
      <div class="item-label">Creativity</div>
    </div>
    <div class="item-card">
      <div class="item-value">∞</div>
      <div class="item-label">Coffee</div>
    </div>
  </div>

  <br><br><br>
  
  <a href="#" class="btn-start">PRESS START</a>
  
</div>

</div>
