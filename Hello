<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Something I Want to Ask You 💖</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      color: #333;
    }
    .card {
      background: white;
      border-radius: 20px;
      padding: 30px;
      max-width: 400px;
      width: 90%;
      box-shadow: 0 20px 40px rgba(0,0,0,0.15);
      text-align: center;
      animation: fadeIn 0.6s ease;
    }
    h1 {
      font-size: 1.5rem;
      margin-bottom: 20px;
    }
    button {
      background: #ff4d6d;
      color: white;
      border: none;
      padding: 12px 20px;
      margin: 10px;
      border-radius: 30px;
      font-size: 1rem;
      cursor: pointer;
      transition: transform 0.2s, background 0.2s;
    }
    button:hover {
      background: #e63956;
      transform: scale(1.05);
    }
    .hidden {
      display: none;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <div class="card">
    <h1 id="question"></h1>
    <div id="buttons"></div>
  </div>  <script>
    const steps = [
      {
        text: "Hey ❤️ Can I ask you something?",
        options: ["Okay 😊"]
      },
      {
        text: "Do you know how happy you make me?",
        options: ["Maybe 🥰", "Tell me 😌"]
      },
      {
        text: "Do you know you’re my favorite person?",
        options: ["Aww 🥹", "Really? 💕"]
      },
      {
        text: "Would you make me the happiest person this Valentine’s Day?",
        options: ["What do you mean? 😳"]
      },
      {
        text: "Will you be my Valentine? 💘",
        options: ["YES!!! 💖", "Of course 😍"]
      },
      {
        text: "Yayyy!!! 💃🌹 Happy Valentine’s Day, my love!",
        options: []
      }
    ];

    let current = 0;
    const questionEl = document.getElementById('question');
    const buttonsEl = document.getElementById('buttons');

    function renderStep() {
      questionEl.textContent = steps[current].text;
      buttonsEl.innerHTML = '';

      steps[current].options.forEach(option => {
        const btn = document.createElement('button');
        btn.textContent = option;
        btn.onclick = () => {
          current++;
          renderStep();
        };
        buttonsEl.appendChild(btn);
      });
    }

    renderStep();
  </script></body>
</html>
