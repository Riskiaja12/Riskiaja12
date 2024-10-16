<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Judi Sederhana</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            text-align: center;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h1 {
            color: #333;
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background-color: #28a745;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Selamat Datang di Website Judi Sederhana</h1>
        <button id="playButton">Mainkan!</button>
        <p id="result"></p>
    </div>

    <script>
        document.getElementById("playButton").onclick = function() {
            const randomNumber = Math.random();
            let result;

            if (randomNumber < 0.5) {
                result = "Kamu Menang!";
            } else {
                result = "Kamu Kalah!";
            }

            document.getElementById("result").innerText = result;
        };
    </script>
</body>
</html>
