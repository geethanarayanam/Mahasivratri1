<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mahashivratri Gift Hub</title>
    <style>
        /* Centers everything on the entire screen */
        body {
            background: radial-gradient(circle, #1a1a2e 0%, #0f0f1a 100%);
            color: #ffffff;
            font-family: 'Arial', sans-serif;
            display: flex;
            justify-content: center; /* Horizontal Center */
            align-items: center;     /* Vertical Center */
            height: 100vh;
            margin: 0;
            overflow: hidden;
        }

        /* The Card Container */
        .gift-card {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 25px;
            padding: 50px 30px;
            width: 90%;
            max-width: 400px;
            
            /* Centers the content inside the card */
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.5);
            transition: all 0.4s ease-in-out;
        }

        .om-icon {
            font-size: 70px;
            color: #f0a500;
            text-shadow: 0 0 15px rgba(240, 165, 0, 0.5);
            margin-bottom: 15px;
        }

        h1 {
            font-size: 1.6rem;
            color: #f0a500;
            margin-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        p {
            color: #d1d1d1;
            font-size: 1rem;
            margin-bottom: 25px;
        }

        /* The Button */
        .reveal-btn {
            background: linear-gradient(45deg, #f0a500, #ffcc00);
            border: none;
            padding: 15px 40px;
            color: #1a1a2e;
            font-size: 1.1rem;
            font-weight: bold;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(240, 165, 0, 0.3);
            transition: 0.3s;
        }

        .reveal-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 25px rgba(240, 165, 0, 0.5);
        }

        /* Hidden Wish Section */
        #blessing-box {
            display: none;
            margin-top: 20px;
            animation: zoomIn 0.8s ease forwards;
        }

        @keyframes zoomIn {
            from { opacity: 0; transform: scale(0.9); }
            to { opacity: 1; transform: scale(1); }
        }

        .wish-text {
            font-size: 1.2rem;
            font-style: italic;
            line-height: 1.5;
            color: #fff;
        }

        .shloka {
            margin-top: 15px;
            font-size: 1.4rem;
            font-weight: bold;
            color: #f0a500;
            display: block;
        }
    </style>
</head>
<body>

    <div class="gift-card">
        <div class="om-icon">🕉️</div>
        <h1>Mahashivratri Blessings</h1>
        <p>A sacred wish is waiting for you...</p>
        
        <button class="reveal-btn" onclick="openGift()">Receive Blessing</button>

        <div id="blessing-box">
            <p class="wish-text">"May Lord Shiva's divine grace be with you today and always."</p>
            <span class="shloka">ॐ नमः शिवाय</span>
        </div>
    </div>

    <script>
        function openGift() {
            // Reveal the content
            document.getElementById('blessing-box').style.display = 'block';
            // Hide the button
            document.querySelector('.reveal-btn').style.display = 'none';
        }
    </script>

</body>
</html>
