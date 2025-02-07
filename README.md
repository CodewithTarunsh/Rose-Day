<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Rose Day, Mahii</title>
    <style>
        body {
            background-color: #ffe6e6;
            text-align: center;
            font-family: 'Arial', sans-serif;
            padding: 20px;
            overflow: hidden;
        }
        .container {
            max-width: 600px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
            position: relative;
            animation: fadeIn 2s ease-in-out;
        }
        h1 {
            color: #d63384;
        }
        p {
            font-size: 18px;
            color: #333;
        }
        .rose-img {
            width: 100px;
            margin: 20px 0;
            transition: transform 0.5s;
        }
        .rose-img:hover {
            transform: scale(1.2);
        }
        .heart-btn {
            background-color: #ff3366;
            color: white;
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            border-radius: 20px;
            cursor: pointer;
            transition: 0.3s;
        }
        .heart-btn:hover {
            background-color: #cc0052;
            transform: scale(1.1);
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes floatingText {
            0% { transform: translateY(0); opacity: 1; }
            50% { transform: translateY(-20px); opacity: 0.8; }
            100% { transform: translateY(0); opacity: 1; }
        }
        .floating-text {
            position: absolute;
            width: 100%;
            font-size: 24px;
            color: #d63384;
            font-weight: bold;
            animation: floatingText 3s infinite ease-in-out;
            z-index: -1;
        }
    </style>
    <script>
        function showMessage() {
            let popup = document.createElement("div");
            popup.innerHTML = "I love you, Mahii! ❤️";
            popup.style.position = "fixed";
            popup.style.top = "50%";
            popup.style.left = "50%";
            popup.style.transform = "translate(-50%, -50%)";
            popup.style.background = "#ff3366";
            popup.style.color = "white";
            popup.style.padding = "20px";
            popup.style.borderRadius = "10px";
            popup.style.boxShadow = "0px 0px 10px rgba(0, 0, 0, 0.2)";
            popup.style.zIndex = "1000";
            document.body.appendChild(popup);
            setTimeout(() => { popup.remove(); }, 2000);
        }
    </script>
</head>
<body>
    <div class="floating-text">I Love You Mahii ❤️ Happy Rose Day! 🌹</div>
    <div class="container">
        <h1>Happy Rose Day, Mahii! 🌹</h1>
        <img src="https://www.pngall.com/wp-content/uploads/5/Red-Rose-PNG-Image.png" alt="Rose" class="rose-img">
        <p>My love, every petal of this rose carries my love for you. I’m sorry for last night, and I hope this day brings a fresh start to our love. You are my forever rose. 🌹❤️</p>
        <button class="heart-btn" onclick="showMessage()">I Love You</button>
    </div>
</body>
</html>
