<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <title>FemmeBox</title>
  <style>
    @font-face {
      font-family: 'FBCaramelApple';
      src: url('FBCaramelApple.ttf') format('truetype');
    }
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Arial', sans-serif;
      color: #4a4a4a;
      text-align: center;
    }
    body {
      background: linear-gradient(135deg, #ffe9f3, #ffe0fb);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 40px 20px;
    }
    header {
      font-family: 'FBCaramelApple', cursive;
      font-size: 3.5rem;
      color: #d81b60;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 15px;
      margin-bottom: 40px;
    }
    header img {
      width: 120px;
      height: 120px;
      border-radius: 25px;
      box-shadow: 0 6px 20px rgba(216, 27, 96, 0.6);
      object-fit: contain;
      background: white;
      padding: 10px;
    }
    .quienes-somos, .integrantes {
      max-width: 720px;
      background: white;
      border-radius: 25px;
      padding: 25px 30px;
      box-shadow: 0 15px 35px rgba(216, 27, 96, 0.15);
      font-size: 1.1rem;
      line-height: 1.5;
      margin-bottom: 45px;
    }
    .integrantes h2 {
      margin-bottom: 20px;
      color: #d81b60;
    }
    .kits-container {
      display: flex;
      flex-wrap: wrap;
      gap: 40px;
      justify-content: center;
      max-width: 960px;
      width: 100%;
    }
    .kit {
      background: white;
      border-radius: 25px;
      width: 350px;
      box-shadow: 0 15px 35px rgba(216, 27, 96, 0.15);
      padding: 30px 25px;
      transition: transform 0.3s ease;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .kit:hover {
      transform: translateY(-10px);
      box-shadow: 0 20px 40px rgba(216, 27, 96, 0.3);
    }
    .kit img.main-img {
      width: 140px;
      height: 140px;
      border-radius: 50%;
      object-fit: cover;
      box-shadow: 0 8px 20px rgba(216, 27, 96, 0.25);
      margin-bottom: 20px;
      transition: transform 0.4s ease;
    }
    .kit:hover img.main-img {
      transform: scale(1.05);
    }
    .kit h3 {
      margin-bottom: 15px;
      font-size: 1.5rem;
      color: #d81b60;
      letter-spacing: 0.05em;
    }
    .video-container {
      margin-top: 15px;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 10px 25px rgba(216, 27, 96, 0.2);
      width: 100%;
    }
    iframe {
      width: 100%;
      height: 180px;
      border: none;
    }
    .info-text {
      margin-top: 15px;
      font-size: 0.9rem;
      line-height: 1.3;
      color: #6a6a6a;
    }
    .ver-mas {
      display: inline-block;
      background: linear-gradient(135deg, #d81b60, #f48fb1);
      color: white;
      font-weight: 600;
      padding: 10px 22px;
      border-radius: 30px;
      font-size: 1rem;
      text-decoration: none;
      box-shadow: 0 6px 15px rgba(216, 27, 96, 0.3);
      transition: background 0.3s ease;
      margin-top: 15px;
      cursor: pointer;
      border: none;
    }
    footer {
      margin-top: 60px;
      width: 100%;
      text-align: center;
      padding: 25px 0;
      background-color: #f8bbd0;
      color: white;
      font-weight: 500;
      letter-spacing: 0.05em;
      border-radius: 20px 20px 0 0;
      box-shadow: 0 -6px 20px rgba(216, 27, 96, 0.2);
    }
  </style>
</head>
<body>

<header>
  <img src="https://i.imgur.com/P3Ij9II.jpg" alt="Logo FemmeBox" />
  FemmeBox - Kits de Bienestar
</header>

<section class="quienes-somos">
  <p><strong>Quiénes somos:</strong> Ofrecemos kits personalizados de productos de cuidado y bienestar según la etapa de la vida de la mujer.</p>
  <p>Porque las mujeres suelen comprar productos de forma separada y sin orientación, lo que es costoso y poco práctico.</p>
  <p>Facilitamos el acceso a productos esenciales, promovemos el autocuidado femenino y brindamos información confiable de salud y bienestar.</p>
</section>

<section class="integrantes">
  <h2>Integrantes</h2>
  <p><strong>Sofia Feng</strong> → Diseñadora del prototipo (app y logotipo).</p>
  <p><strong>Piero Lopez</strong> → Encargado de kits (armar ejemplos de productos).</p>
  <p><strong>Dhanna Rojas</strong> → Marketing y comunicación (difusión en el colegio).</p>
</section>

<div class="kits-container">

  <!-- KITS ORIGINALES -->

  <!-- Kit 4 Bienestar Juvenil -->
  <div class="kit">
    <img src="https://i.imgur.com/ze21zby.jpg" alt="Kit Juvenil" class="main-img" />
    <h3>Kit de Bienestar Juvenil</h3>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/dZiJp76DLe4" allowfullscreen></iframe>
    </div>
    <div class="info-text">Productos esenciales para jóvenes que comienzan a cuidar su cuerpo y bienestar.</div>
    <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
    <div class="extra-content">
      <ol class="products-list">
        <li>Gel facial suave</li>
        <li>Desodorante natural</li>
        <li>Toallitas reutilizables</li>
        <li>Agenda de autocuidado</li>
        <li>Mini espejo portátil</li>
        <li>Estuche organizador</li>
      </ol>
    </div>
  </div>

  <!-- Kit 5 Autoestima -->
  <div class="kit">
    <img src="https://i.imgur.com/NUegUh8.jpg" alt="Kit Autoestima" class="main-img" />
    <h3>Kit Autoestima y Cuidado Personal</h3>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/LWeWviJJHoo" allowfullscreen></iframe>
    </div>
    <div class="info-text">Fortalece el amor propio y bienestar emocional.</div>
    <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
  </div>

  <!-- Kit 6 Salud Deportiva -->
  <div class="kit">
    <img src="https://i.imgur.com/Vk3RsVp.jpg" alt="Kit Salud Deportiva" class="main-img" />
    <h3>Kit Salud Deportiva</h3>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/YWY_9y05HBU" allowfullscreen></iframe>
    </div>
    <div class="info-text">Complemento ideal para la actividad física.</div>
    <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
  </div>

  <!-- Kit 7 Relajación -->
  <div class="kit">
    <img src="https://i.imgur.com/BGlMJPw.jpg" alt="Kit Spa" class="main-img" />
    <h3>Kit Relajación y Spa</h3>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/VvqvDKRbgvY" allowfullscreen></iframe>
    </div>
    <div class="info-text">Para desconectar y relajarse desde casa.</div>
    <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
  </div>

  <!-- Kit 8 Salud Mental -->
  <div class="kit">
    <img src="https://i.imgur.com/n1LFtB6.jpg" alt="Kit Salud Mental" class="main-img" />
    <h3>Kit Salud Mental y Equilibrio</h3>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/UpGV7QXKzPI" allowfullscreen></iframe>
    </div>
    <div class="info-text">Bienestar emocional y manejo del estrés.</div>
    <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
  </div>

  <!-- Kit 9 Cuidado Nocturno -->
  <div class="kit">
    <img src="https://i.imgur.com/MfODBjN.jpg" alt="Kit Nocturno" class="main-img" />
    <h3>Kit Cuidado Nocturno</h3>
    <div class="video-container">
      <iframe src="https://www.youtube.com/embed/eKjIgG0xuU8" allowfullscreen></iframe>
    </div>
    <div class="info-text">Rutinas relajantes para dormir mejor.</div>
    <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
  </div>

</div>

<footer>
  <p>&copy; 2024 FemmeBox | Todos los derechos reservados.</p>
</footer>

<script>
  function toggleContent(button) {
    const content = button.nextElementSibling;
    if (content.style.display === "block") {
      content.style.display = "none";
      button.textContent = "Ver más";
    } else {
      content.style.display = "block";
      button.textContent = "Ver menos";
    }
  }
</script>

</body>
</html>


