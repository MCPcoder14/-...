<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Скоро здесь будет мой первый сайт</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            display: flex;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            font-family: 'Segoe UI', Tahoma, sans-serif;
            color: #fff;
            overflow: hidden;
        }

        .container {
            text-align: center;
            padding: 40px;
            position: relative;
        }

        .glow {
            position: absolute;
            top: 50%;
            left: 50%;
            width: 400px;
            height: 400px;
            background: radial-gradient(circle, rgba(120, 80, 255, 0.3), transparent 70%);
            transform: translate(-50%, -50%);
            animation: pulse 4s ease-in-out infinite;
            border-radius: 50%;
        }

        h1 {
            font-size: clamp(1.8rem, 5vw, 3.2rem);
            font-weight: 700;
            margin-bottom: 16px;
            background: linear-gradient(90deg, #a78bfa, #60a5fa, #a78bfa);
            background-size: 200% auto;
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: shine 4s linear infinite;
            position: relative;
        }

        p {
            font-size: clamp(1rem, 2.5vw, 1.25rem);
            opacity: 0.8;
            letter-spacing: 0.5px;
            animation: fadeIn 1.5s ease-out;
        }

        .dots span {
            display: inline-block;
            animation: bounce 1.4s infinite ease-in-out;
            opacity: 0.6;
        }

        .dots span:nth-child(1) { animation-delay: 0s; }
        .dots span:nth-child(2) { animation-delay: 0.2s; }
        .dots span:nth-child(3) { animation-delay: 0.4s; }

        @keyframes pulse {
            0%, 100% { transform: translate(-50%, -50%) scale(1); opacity: 0.6; }
            50% { transform: translate(-50%, -50%) scale(1.15); opacity: 1; }
        }

        @keyframes shine {
            to { background-position: 200% center; }
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 0.8; transform: translateY(0); }
        }

        @keyframes bounce {
            0%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-8px); }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="glow"></div>
        <h1>Скоро здесь будет мой первый сайт</h1>
        <p>Уже работаю над этим<span class="dots"><span>.</span><span>.</span><span>.</span></span></p>
    </div>
</body>
</html>
