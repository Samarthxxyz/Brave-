<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>To the Brave and the Bright</title>
  <style>
    /* Page Styling */
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: radial-gradient(ellipse at bottom, #1b2735 0%, #090a0f 100%);
      overflow: hidden;
      color: white;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      height: 100vh;
      padding: 20px;
    }

    /* Star Background Animation */
    .stars {
      position: absolute;
      width: 100%;
      height: 100%;
      background: url('https://media.giphy.com/media/l0HUpt2s9Pclgt9Vm/giphy.gif') repeat;
      background-size: cover;
      opacity: 0.15;
      z-index: 0;
    }

    /* Content Box */
    .content {
      position: relative;
      z-index: 1;
      max-width: 800px;
      padding: 30px;
      background: rgba(255, 255, 255, 0.05);
      border-radius: 16px;
      box-shadow: 0 0 20px rgba(0,0,0,0.4);
    }

    h1 {
      font-size: 2.8em;
      margin-bottom: 0.5em;
      color: #00ffd5;
      text-shadow: 0 0 10px #00ffd5, 0 0 30px #00ffd5;
      animation: glow 2s ease-in-out infinite alternate;
    }

    @keyframes glow {
      from {
        text-shadow: 0 0 5px #00ffd5;
      }
      to {
        text-shadow: 0 0 20px #00ffd5, 0 0 30px #00ffd5;
      }
    }

    p {
      font-size: 1.2em;
      color: #cce7ff;
      margin-bottom: 1.5em;
    }

    button {
      background-color: #00ffd5;
      color: #002f40;
      padding: 12px 24px;
      font-size: 1em;
      font-weight: bold;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: #00c9a7;
    }

    .secret {
      display: none;
      margin-top: 30px;
      font-size: 1.1em;
      color: #fff;
      background: rgba(0, 255, 213, 0.1);
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }

    .footer {
      margin-top: 30px;
      font-size: 0.95em;
      color: #88aabb;
      font-style: italic;
    }
  </style>
</head>
<body>
  <div class="stars"></div>

  <div class="content">
    <h1>To the Brave and the Bright</h1>
    <p>
      This space is a quiet tribute.<br>
      For the courage of those who serve.<br>
      And the light of those who inspire.
    </p>
    <button onclick="document.querySelector('.secret').style.display='block'">Click to Reveal</button>
    <div class="secret">
      Maybe you don’t know yet, but someone out there holds you in the highest respect.<br>
      Your strength, your grace, and your world mean more than words can ever say.<br>
      One day, when the moment is right, the truth will find its way — gently.
    </div>
    <div class="footer">
      — With strength, silence, and hope
    </div>
  </div>
</body>
</html>
