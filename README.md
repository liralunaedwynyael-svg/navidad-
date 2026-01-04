<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Cómpramelo para que juguemos</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            background: linear-gradient(#0b3d2e, #145a32);
            color: white;
            text-align: center;
            overflow-x: hidden;
        }

        h1 {
            margin-top: 40px;
            font-size: 3.2em;
            text-shadow: 2px 2px 5px #000;
        }

        .container {
            margin-top: 60px;
        }

        .btn {
            display: inline-block;
            margin-top: 30px;
            padding: 20px 35px;
            font-size: 1.4em;
            background-color: #c0392b;
            color: white;
            text-decoration: none;
            border-radius: 15px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.4);
            transition: transform 0.2s, background-color 0.2s;
        }

        .btn:hover {
            background-color: #e74c3c;
            transform: scale(1.05);
        }

        .snowflake {
            position: fixed;
            top: -10px;
            color: white;
            font-size: 1em;
            animation: fall linear infinite;
        }

        @keyframes fall {
            to {
                transform: translateY(110vh);
            }
        }

        footer {
            margin-top: 80px;
            font-size: 0.9em;
            opacity: 0.8;
        }
    </style>
</head>
<body>

    <h1>🎄 Cómpramelo para que juguemos 🎮</h1>

    <div class="container">
        <p style="font-size:1.3em;">Haz clic y vamos a divertirnos juntos 😄</p>

        <a class="btn" href="https://www.mercadolibre.com.mx/p/MLM19610178?pdp_filters=item_id:MLM2610463427#origin=share&sid=share&wid=MLM2610463427&action=whatsapp" target="_blank">
            🎁 Ver en Mercado Libre
        </a>
    </div>

    <footer>
        ❄️ Hecho con espíritu navideño ❄️
    </footer>

    <script>
        function crearNieve() {
            const snowflake = document.createElement("div");
            snowflake.className = "snowflake";
            snowflake.innerHTML = "❄";
            snowflake.style.left = Math.random() * window.innerWidth + "px";
            snowflake.style.animationDuration = (Math.random() * 3 + 2) + "s";
            snowflake.style.fontSize = (Math.random() * 10 + 10) + "px";
            document.body.appendChild(snowflake);

            setTimeout(() => {
                snowflake.remove();
            }, 5000);
        }

        setInterval(crearNieve, 200);
    </script>

</body>
</html>
