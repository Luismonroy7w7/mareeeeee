<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Me amas?</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            height: 100%;
            background-color: #ffd6ec;
            font-family: Arial, sans-serif;
        }

        .container {
            background-color: #FFFFFF;
            width: 80%;
            height: auto;
            padding: 2em;
            border: 1px solid;
            border-radius: 20px;
            text-align: center;
            margin: auto;
        }

        .slides {
            display: none;
        }

        .slides img {
            max-width: 90%;
            height: auto;
            border-radius: 8px;
            margin: 0 auto;
        }

        .slides p {
            font-size: 25px;
            color: #333;
            margin: 10px 0;
        }

        label {
            background-color: #FF8585;
            color: #FFFFFF;
            padding: 10px 20px;
            margin: 25px 0;
            border-radius: 20px;
            display: inline-block;
            cursor: pointer;
            font-size: 34px;
            border: 1px solid black;
            width: 200px;
            height: auto;
            filter: drop-shadow(2px 4px 6px black);
        }

        .disabled {
            background-color: grey;
            filter: none;
            pointer-events: none;
            opacity: 0.5;
        }

        @media (max-width: 600px) {
            label {
                width: 90%;
                padding: 15px;
                font-size: 34px;
            }
        }

        #slide1:checked~.container #foto1,
        #slide2:checked~.container #foto2 {
            display: block;
        }
    </style>
</head>
<body>
    <input type="radio" name="slides" id="slide1" checked>
    <input type="radio" name="slides" id="slide2">

    <div class="container">
        <div id="foto1" class="slides">
            <div>
                <p>¿Me amas?</p>
            </div>
            <div style="display: flex; justify-content: space-evenly;">
                <label for="slide2">Sí</label>
                <label class="disabled">No</label>
            </div>
            <div style="display: flex; justify-content: center;">
                <img width="600px" height="700px" style="border-radius: 10px;" src="rata flores.jpg" alt="Gato 1">
            </div>
        </div>

        <div id="foto2" class="slides">
            <p>❤️yo ti amo musho más❤️</p>
            <div style="display: flex; justify-content: center;">
                <img width="600px" height="700px" style="border-radius: 10px;" src="rata feliz.jpg" alt="Gato 2">
            </div>
        </div>
    </div>
</body>
</html>

