<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Daniela y Anthony</title>
    <style>
        body {
            background-color: #E6E6FA;
            background-image: url('hearts-background.png'); /* Aquí puedes poner una imagen de fondo con corazones */
            background-repeat: repeat;
            text-align: center;
            font-family: Arial, sans-serif;
            color: #000;
            overflow: hidden;
        }
        .container {
            position: relative;
            display: inline-block;
            margin-top: 50px;
        }
        .text {
            font-size: 24px;
            background: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
            padding: 20px;
            display: inline-block;
        }
        .rose {
            width: 100px;
            position: relative;
            top: 20px;
        }
        .petal {
            position: absolute;
            background-color: red;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            opacity: 0.8;
            animation: fall 5s linear infinite;
        }
        @keyframes fall {
            0% { top: 0; opacity: 0.8; }
            100% { top: 500px; opacity: 0; }
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="rose.png" alt="Rosa" class="rose" id="rose">
        <div class="text">
            Siempre estaré en las buenas y las malas, siempre cuenta conmigo para lo que sea mi ardilla hermosa. Eres la niña que me provoca hacerte estos detalles.
        </div>
    </div>
    <script>
        const rose = document.getElementById('rose');
        const container = document.querySelector('.container');

        function createPetal() {
            const petal = document.createElement('div');
            petal.classList.add('petal');
            petal.style.left = Math.random() * rose.offsetWidth + 'px';
            container.appendChild(petal);

            petal.addEventListener('animationend', () => {
                petal.remove();
            });
        }

        setInterval(createPetal, 300);
    </script>
</body>
</html>
- 👋 Hi, I’m @ANTHONY4444MM
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
ANTHONY4444MM/ANTHONY4444MM is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
