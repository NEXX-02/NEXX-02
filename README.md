<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nexx Payment</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

        body {
            margin: 0;
            padding: 0;
            background-color: #0d0d0d;
            color: white;
            font-family: 'Roboto', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: radial-gradient(circle at top left, #1a2a6c, #b21f1f, #fdbb2d);
            overflow: hidden;
        }

        .container {
            background-color: rgba(0, 0, 0, 0.85);
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.6);
            text-align: center;
            position: relative;
            max-width: 350px;
            width: 100%;
        }

        h1 {
            font-size: 32px;
            margin-bottom: 20px;
            color: #fdbb2d;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .qr-container {
            margin-bottom: 20px;
        }

        .qr-container img {
            width: 100%;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            transition: transform 0.5s ease;
        }

        .qr-container img:hover {
            transform: scale(1.05);
        }

        .payment-info {
            font-size: 18px;
            margin-bottom: 20px;
            color: #e0e0e0;
        }

        .button {
            display: inline-block;
            padding: 12px 25px;
            font-size: 18px;
            color: #fff;
            text-decoration: none;
            border-radius: 30px;
            background: linear-gradient(135deg, #1a2a6c, #b21f1f);
            transition: background 0.5s ease, transform 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        .button:hover {
            background: linear-gradient(135deg, #fdbb2d, #b21f1f);
            transform: scale(1.05);
        }

        .floating-elements {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
        }

        .floating-elements img {
            position: absolute;
            animation: float 15s infinite;
            opacity: 0.15;
            width: 80px;
            height: 80px;
        }

        @keyframes float {
            0% {
                transform: translateY(0) rotate(0deg);
            }
            50% {
                transform: translateY(-20px) rotate(360deg);
            }
            100% {
                transform: translateY(0) rotate(720deg);
            }
        }

        .element1 {
            top: 10%;
            left: 20%;
        }

        .element2 {
            top: 60%;
            left: 80%;
        }

        .element3 {
            top: 30%;
            left: 60%;
        }
    </style>
</head>
<body>
    <div class="floating-elements">
        <img src="https://cdn-icons-png.flaticon.com/512/616/616490.png" class="element1" alt="Floating Icon">
        <img src="https://cdn-icons-png.flaticon.com/512/616/616490.png" class="element2" alt="Floating Icon">
        <img src="https://cdn-icons-png.flaticon.com/512/616/616490.png" class="element3" alt="Floating Icon">
    </div>
    <div class="container">
        <h1>Nexx Payment</h1>
        <div class="qr-container">
            <img src="your_qr_code_image_path.jpg" alt="Nexx QR Code">
        </div>
        <p class="payment-info">Scan the QR code to make a payment</p>
        <p class="payment-info">UPI ID: 9871363778@fam</p>
        <a href="#" class="button">Make Payment</a>
    </div>
</body>
</html>
