<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <title>Cartão de Visita - Tintim</title>
    <style>
        @font-face {
            font-family: 'TintinFont';
            src: url("{{ url_for('static', filename='tintimarm.png') }}");
        }

        body {
            background-color: #df1313; /* azul claro estilo blusa do Tintim */
            font-family: 'TintinFont', Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .cartao {
            background-color: #faf0f0;
            border: 4px solid #050404;
            border-radius: 15px;
            box-shadow: 5px 5px 0 #444;
            padding: 30px;
            text-align: center;
            width: 400px;
            position: relative;
        }

        .cartao img {
            width: 130px;
            height: 130px;
            border-radius: 50%;
            border: 3px solid #000;
            object-fit: cover;
            margin-bottom: 15px;
        }

        .cartao h1 {
            font-size: 26px;
            margin-bottom: 5px;
            color: #1c1c1c;
        }

        .cartao p {
            font-size: 15px;
            color: #333;
            margin: 5px 0;
        }

        .contato {
            margin-top: 15px;
        }

        .contato p {
            font-size: 14px;
        }

        .milu {
            position: absolute;
            bottom: -20px;
            right: -20px;
            width: 60px;
        }
    </style>
</head>
<body>
    <div class="cartao">
        <img src="{{ url_for('static', filename='tintimarm.png') }}" alt="Tintim">
        <h1>Tintim do morro </h1>
        <p>Repórter Aventureiro</p>
        <div class="contato">
            <p>📧 tintim@exploradores.com</p>
            <p>📞 +11  456 789 000</p>
            <h2>  Milu </h2>
        </div>
        <img class="milu" src="{{ url_for('static', filename='milu.png') }}" alt="Milu">
    </div>
</body>
</html>
