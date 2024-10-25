[Uploading 8th 2 .html…]()<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>3D Rotating Heart with Infinity Symbol</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #000;
            color: #fff;
            margin: 0;
            text-align: center;
        }

        h1 {
            color: #FFD700; /* Gold */
            margin-bottom: 20px;
        }

        h4 {
            color: #FF69B4; /* Hot Pink */
            margin-bottom: 20px;
        }

        .heart {
            position: relative;
            width: 150px;
            height: 150px;
            background-color: red;
            transform: rotate(-45deg);
            margin: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            animation: rotate3D 5s infinite linear;
        }

        .heart:before,
        .heart:after {
            content: '';
            position: absolute;
            width: 150px;
            height: 150px;
            background-color: red;
            border-radius: 50%;
        }

        .heart:before {
            top: -75px;
            left: 0;
        }

        .heart:after {
            left: 75px;
            top: 0;
        }

        .infinity-symbol {
            position: absolute;
            width: 80px;
            height: 40px;
            background: transparent;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .infinity-symbol:before,
        .infinity-symbol:after {
            content: '';
            position: absolute;
            width: 40px;
            height: 40px;
            border: 5px solid #FF69B4; /* Hot Pink */
            border-radius: 50%;
        }

        .infinity-symbol:before {
            left: 0;
            transform: rotate(45deg);
        }

        .infinity-symbol:after {
            right: 0;
            transform: rotate(45deg);
        }

        .infinity-symbol::before,
        .infinity-symbol::after {
            box-shadow: 0 0 15px rgba(255, 105, 180, 0.7);
        }

        @keyframes rotate3D {
            0% {
                transform: rotateY(0deg) rotate(-45deg);
            }
            50% {
                transform: rotateY(180deg) rotate(-45deg);
            }
            100% {
                transform: rotateY(360deg) rotate(-45deg);
            }
        }

    </style>
</head>
<body>

    <h1>Hello BB, Kiss sa ko bi, Mwah!</h1>
    <h4>So, since we're getting to our 8th monthsary, I wanna make you this thing hehe.</h4>
    <div class="heart">
        <div class="infinity-symbol"></div>
    </div>
    <h4>I LOVE YOU ALWAYS B</h4>

</body>
</html>

