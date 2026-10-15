<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Cute Corner ✨</title>
    <style>
        /* Soft, warm pastel background */
        body {
            background-color: #eef7ff; /* Sky Blue */
            font-family: 'Quicksand', 'Segoe UI', sans-serif;
            color: #6c5b7b;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
        }

        /* Cute main container */
        .card {
            background: #ffffff;
            border: 4px solid #ffb6c1; /* Light Pink Border */
            border-radius: 24px;
            box-shadow: 0 8px 24px rgba(255, 182, 193, 0.4);
            padding: 30px;
            max-width: 400px;
            width: 90%;
            text-align: center;
            transition: transform 0.3s ease;
        }

        /* Soft float effect when hovering over the card */
        .card:hover {
            transform: translateY(-5px);
        }

        /* Sparkly header */
        h1 {
            color: #ff6b8b;
            font-size: 2rem;
            margin-bottom: 10px;
        }

        p {
            font-size: 1.1rem;
            line-height: 1.6;
            margin-bottom: 20px;
        }

        /* Cute round button with bouncy hover animation */
        .cute-btn {
            background-color: #ffb6c1;
            color: white;
            border: none;
            padding: 12px 28px;
            font-size: 1rem;
            font-weight: bold;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(255, 182, 193, 0.5);
            transition: all 0.2s ease-in-out;
        }

        .cute-btn:hover {
            background-color: #ff6b8b;
            transform: scale(1.05);
        }
        
        .sparkles {
            color: #ffd700;
        }
    </style>
</head>
<body>

    <div class="card">
        <h1>Hello LSMG FAN! <span class="sparkles">✨</span></h1>
        <p>Welcome to my cozy digital space. I'm coding interactive layouts using sweet pastel accents, soft drop shadows, and bouncy transitions.</p>
        <button class="cute-btn" onclick="alert('Yay! Thanks for visiting! 💕')">Click Me! 🐾</button>
    </div>

</body>
</html>
