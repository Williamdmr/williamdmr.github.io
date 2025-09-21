<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Flor Amarilla</title>
  <style>
    body {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      background: #fdf6e3;
      font-family: Arial, sans-serif;
    }

    button {
      padding: 12px 20px;
      font-size: 18px;
      border: none;
      border-radius: 8px;
      background: #ffcc00;
      cursor: pointer;
      box-shadow: 0 4px 6px rgba(0,0,0,0.2);
    }

    button:hover {
      background: #ffdb4d;
    }

    .flor {
      margin-top: 30px;
      width: 150px;
      height: 150px;
      position: relative;
      display: none;
    }

    .petalo {
      width: 80px;
      height: 80px;
      background: yellow;
      border-radius: 50%;
      position: absolute;
    }

    .petalo:nth-child(1) { top: 0; left: 35px; }
    .petalo:nth-child(2) { top: 35px; left: 0; }
    .petalo:nth-child(3) { top: 35px; right: 0; }
    .petalo:nth-child(4) { bottom: 0; left: 35px; }

    .centro {
      width: 70px;
      height: 70px;
      background: orange;
      border-radius: 50%;
      position: absolute;
      top: 40px;
      left: 40px;
    }
  </style>
</head>
<body>
  <button onclick="mostrarFlor()">🌼 Mostrar Flor</button>

  <div class="flor" id="flor">
    <div class="petalo"></div>
    <div class="petalo"></div>
    <div class="petalo"></div>
    <div class="petalo"></div>
    <div class="centro"></div>
  </div>

  <script>
    function mostrarFlor() {
      document.getElementById("flor").style.display = "block";
    }
  </script>
</body>
</html>
