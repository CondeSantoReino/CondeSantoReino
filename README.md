<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Número Par Aleatorio</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: Arial, sans-serif;
            background-color: #f0f8ff;
            margin: 0;
        }
        .container {
            text-align: center;
        }
        #randomNumber {
            font-size: 2em;
            color: #333;
            margin: 20px 0;
        }
        #generateButton {
            padding: 10px 20px;
            font-size: 1em;
            color: #fff;
            background-color: #4CAF50;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        #generateButton:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Generador de Números Pares Aleatorios</h1>
        <div id="randomNumber">Haz clic en el botón</div>
        <button id="generateButton" onclick="generateEvenNumber()">Generar Número Par</button>
    </div>

    <script>
        function generateEvenNumber() {
            // Genera un número par aleatorio entre 1 y 1,000,000,000,000
            const min = 2;
            const max = 1000000000000;
            
            // Genera un número aleatorio par en el rango
            const randomEvenNumber = Math.floor(Math.random() * ((max - min) / 2 + 1)) * 2 + min;
            
            document.getElementById("randomNumber").textContent = randomEvenNumber;
        }
    </script>
</body>
</html>
