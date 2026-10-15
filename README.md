<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cute Aesthetic Card ✨</title>
    <style>
        /* Import a rounded, playful font */
        @import url('https://googleapis.com');

        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #ffeef2; /* Soft pastel pink background */
            font-family: 'Fredoka', sans-serif;
            overflow: hidden;
        }

        /* Floating background shapes for extra cuteness */
        .bubble {
            position: absolute;
            background-color: rgba(255, 255, 255, 0.6);
            border-radius: 50%;
            animation: floatUp 8s infinite ease-in-out;
            z-index: 1;
        }

        /* Main aesthetic container */
        .card {
            background-color: #ffffff;
            border: 4px solid #ffb7c5;
            border-radius: 30px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 12px 24px rgba(255, 183, 197, 0.4);
            max-width: 350px;
            width: 90%;
            z-index: 10;
            position: relative;
            transform: translateY(0px);
            animation: gentleHover 4s infinite ease-in-out;
        }

        /* Mascot character styling */
        .mascot-container {
            font-size: 80px;
            margin-bottom: 15px;
            display: inline-block;
            animation: bounce 2s infinite ease-in-out;
        }

        h1 {
            color: #ff6584;
            font-size: 28px;
            margin: 10px 0;
        }

        p {
            color: #7d6b6f;
            font-size: 16px;
            line-height: 1.5;
            margin-bottom: 25px;
        }

        /* Interactive pulse button */
        .cute-btn {
            background-color: #ff6584;
            color: white;
            border: none;
            border-radius: 50px;
            padding: 12px 30px;
            font-size: 18px;
            font-family: 'Fredoka', sans-serif;
            font-weight: 600;
            cursor: pointer;
            box-shadow: 0 6px 0 #d94563;
            transition: all 0.1s ease;
            outline: none;
        }

        .cute-btn:hover {
            background-color: #ff7e99;
            transform: translateY(2px);
            box-shadow: 0 4px 0 #d94563;
        }

        .cute-btn:active {
            transform: translateY(6px);
            box-shadow: 0 0px 0 #d94563;
        }

        /* Sparkles and falling elements */
        .confetti {
            position: absolute;
            font-size: 20px;
            animation: fall 3s linear forwards;
            pointer-events: none;
            z-index: 100;
        }

        /* Animations */
        @keyframes gentleHover {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0) scale(1); }
            50% { transform: translateY(-8px) scale(1.05); }
        }

        @keyframes floatUp {
            0% { transform: translateY(100vh) translateX(0); opacity: 0; }
            10% { opacity: 1; }
            90% { opacity: 1; }
            100% { transform: translateY(-10vh) translateX(50px); opacity: 0; }
        }

        @keyframes fall {
            0% { transform: translateY(-20px) rotate(0deg); opacity: 1; }
            100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
        }
    </style>
</head>
<body>

    <!-- Soft background decorations -->
    <div class="bubble" style="width: 40px; height: 40px; left: 10%; animation-delay: 0s;"></div>
    <div class="bubble" style="width: 60px; height: 60px; left: 80%; animation-delay: 2s;"></div>
    <div class="bubble" style="width: 30px; height: 30px; left: 70%; animation-delay: 5s;"></div>

    <!-- The Cute Card -->
    <div class="card">
        <div class="mascot-container">🐻</div>
        <h1>Hello, Pookie!</h1>
        <p>You have successfully stumbled upon a tiny cozy corner of the web. Click the heart to send some love!</p>
        <button class="cute-btn" onclick="spreadLove()">Press Me 💖</button>
    </div>

    <script>
        // Fun interaction script
        function spreadLove() {
            const emojis = ['💖', '✨', '🌸', '🐾', '🎀', '🎈'];
            
            for (let i = 0; i < 20; i++) {
                setTimeout(() => {
                    const confetti = document.createElement('div');
                    confetti.classList.add('confetti');
                    
                    // Randomize emoji, horizontal start position, and animation duration
                    confetti.innerText = emojis[Math.floor(Math.random() * emojis.length)];
                    confetti.style.left = Math.random() * 100 + 'vw';
                    confetti.style.animationDuration = (Math.random() * 2 + 2) + 's';
                    
                    document.body.appendChild(confetti);
                    
                    // Clean up elements afterward
                    setTimeout(() => {
                        confetti.remove();
                    }, 4000);
                }, i * 50); // Slight stagger effect
            }
        }
    </script>
</body>
</html>

