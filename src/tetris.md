<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tetris</title>
    <style>
        body { display: flex; justify-content: center; align-items: center; height: 100vh; background: #000; }
        canvas { border: 1px solid #fff; }
    </style>
</head>
<body>
    <canvas id="tetris" width="240" height="400"></canvas>
    <script>
        const canvas = document.getElementById('tetris');
        const context = canvas.getContext('2d');
        context.scale(20, 20);

        function draw() {
            context.clearRect(0, 0, canvas.width, canvas.height);
            // Aquí iría la lógica de dibujado de Tetris.
        }

        function update() {
            draw();
            requestAnimationFrame(update);
        }

        update();
    </script>
</body>
</html>
