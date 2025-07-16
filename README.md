
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ayuda TEMU Gratis</title>
  <style>
    body {
      font-family: sans-serif;
      text-align: center;
      padding: 40px;
      background: linear-gradient(#fefefe, #ffe0e0);
    }
    .boton {
      background-color: #FF5722;
      color: white;
      padding: 15px 30px;
      font-size: 20px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }
    .boton:hover {
      background-color: #E64A19;
    }
    .contador {
      margin-top: 30px;
      font-size: 18px;
      color: #555;
    }
  </style>
</head>
<body>
  <h1>🎁 ¡Ayúdame a ganar un regalo en TEMU!</h1>
  <p>Haz clic en el botón y visita mi enlace de invitación:</p>
  <a href="https://temu.com/s/1ZtKrlvBxl5MY5Rj" target="_blank">
    <button class="boton">✨ Ayudar ahora</button>
  </a>
  <p>¡Gracias por tu apoyo! 🙏</p>

  <div class="contador">
    Esta página ha sido visitada <span id="visitas">...</span> veces.
  </div>

  <script>
    fetch('https://api.countapi.xyz/update/temu-ayuda/contador-visitas/?amount=1')
      .then(res => res.json())
      .then(data => {
        document.getElementById('visitas').textContent = data.value;
      });
  </script>
</body>
</html>