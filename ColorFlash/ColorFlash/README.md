Proyecto visual que cambia colores automáticamente.
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Color Flash</title>
<style>
  body {
    margin: 0;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: sans-serif;
    color: white;
    font-size: 2em;
    transition: background-color 0.5s;
  }
</style>
</head>
<body>
  🎨 ¡Flashea conmigo!
<script>
  function randomColor() {
    return '#' + Math.floor(Math.random()*16777215).toString(16);
  }

  setInterval(() => {
    document.body.style.backgroundColor = randomColor();
  }, 1000);
</script>
</body>
</html>
