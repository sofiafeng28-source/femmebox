<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>FemmeBox - Kits de Bienestar</title>
  <style>
    /* Estilos generales */
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #ff4081;
      color: white;
      text-align: center;
      padding: 20px;
    }
    .kits-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 20px;
    }
    .kit {
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      margin: 10px;
      width: 300px;
      text-align: center;
      padding: 20px;
    }
    .kit img {
      width: 100%;
      height: auto;
      border-radius: 10px;
    }
    .kit h3 {
      color: #ff4081;
      margin-top: 10px;
    }
    .kit p {
      color: #555;
      font-size: 14px;
    }
    .kit button {
      background-color: #ff4081;
      color: white;
      border: none;
      padding: 10px;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 10px;
    }
    .kit button:hover {
      background-color: #e040fb;
    }
    footer {
      background-color: #ff4081;
      color: white;
      text-align: center;
      padding: 20px;
      position: fixed;
      bottom: 0;
      width: 100%;
    }
    footer .social-icons {
      margin-top: 10px;
    }
    footer .social-icons a {
      margin: 0 10px;
    }
    footer .social-icons img {
      width: 30px;
      height: 30px;
      border-radius: 50%;
      object-fit: cover;
    }
  </style>
</head>
<body>

  <header>
    <h1>FemmeBox - Kits de Bienestar</h1>
  </header>

  <div class="kits-container">
    <!-- Ejemplo de un kit -->
    <div class="kit">
      <img src="https://i.imgur.com/rbGqFUv.jpg" alt="Kit de Bienestar">
      <h3>Kit Bienestar</h3>
      <p>Descripción breve del kit.</p>
      <button>Ver más</button>
    </div>
    <!-- Puedes agregar más kits aquí -->
  </div>

  <footer>
    <p>Contacto: +51 934 172 944</p>
    <div class="social-icons">
      <a href="https://www.instagram.com/femmebox_oficial?igsh=MXQyc2VxN3dpdmkzYQ==" target="_blank">
        <img src="https://i.imgur.com/73Waibk.jpg" alt="Instagram">
      </a>
      <a href="https://wa.me/51934172944" target="_blank">
        <img src="https://i.imgur.com/SdduDqI.jpg" alt="WhatsApp">
      </a>
    </div>
  </footer>

</body>
</html>


