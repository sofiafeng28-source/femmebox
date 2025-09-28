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
      text-align: center;
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
      color: #555;
      font-size: 1.1rem;
      line-height: 1.5;
      margin-bottom: 45px;
      margin-left: auto;
      margin-right: auto;
      text-align: center;
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
      text-align: center;
    }
    .kit {
      background: white;
      border-radius: 25px;
      width: 350px;
      box-shadow: 0 15px 35px rgba(216, 27, 96, 0.15);
      padding: 30px 25px;
      transition: transform 0.3s ease;
      position: relative;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
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
      text-align: center;
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
    .ver-mas:hover {
      background: linear-gradient(135deg, #f48fb1, #d81b60);
    }
    .extra-content {
      margin-top: 15px;
      font-size: 0.9rem;
      color: #505050;
      text-align: left;
      max-height: 0;
      overflow: hidden;
      transition: max-height 0.5s ease;
    }
    .extra-content.active {
      max-height: 600px;
    }
    .testimonials {
      background: #fff0f5;
      border-radius: 15px;
      padding: 15px 20px;
      margin-top: 20px;
      font-style: italic;
      color: #a63d60;
      font-size: 0.95rem;
      text-align: center;
    }
    ol.products-list {
      list-style-type: decimal;
      padding-left: 20px;
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
    .social-icons {
      margin-top: 12px;
    }
    .social-icons a {
      margin: 0 15px;
      display: inline-block;
      transition: transform 0.2s ease;
    }
    .social-icons a:hover {
      transform: scale(1.15);
    }
    .social-icons img {
      width: 38px;
      height: 38px;
      filter: drop-shadow(0 2px 4px rgba(216, 27, 96, 0.5));
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

    <!-- Kit 1: Adolescencia -->
    <div class="kit">
      <img src="https://i.imgur.com/ze21zby.jpg" alt="Adolescencia" class="main-img" />
      <h3>Kit Adolescencia</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/dZiJp76DLe4" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Productos esenciales para acompañar el inicio del autocuidado en la etapa adolescente.
      </div>
    </div>

    <!-- Kit 2: Cuidado de Piel -->
    <div class="kit">
      <img src="https://i.imgur.com/MfODBjN.jpg" alt="Cuidado de Piel" class="main-img" />
      <h3>Kit Cuidado de Piel</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/eKjIgG0xuU8" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Artículos pensados para mantener la piel limpia, hidratada y protegida.
      </div>
    </div>

    <!-- Kit 3: Postparto -->
    <div class="kit">
      <img src="https://i.imgur.com/n1LFtB6.jpg" alt="Postparto" class="main-img" />
      <h3>Kit Postparto</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/UpGV7QXKzPI" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Productos pensados para el bienestar y recuperación después del parto.
      </div>
    </div>

        <!-- Kit 4: Bienestar Emocional -->
    <div class="kit">
      <img src="https://i.imgur.com/NUegUh8.jpg" alt="Bienestar Emocional" class="main-img" />
      <h3>Kit Bienestar Emocional</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/LWeWviJJHoo" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Pensado para fortalecer el amor propio y la salud emocional con productos prácticos.
      </div>
    </div>

    <!-- Kit 5: Fitness y Salud -->
    <div class="kit">
      <img src="https://i.imgur.com/BGlMJPw.jpg" alt="Fitness y Salud" class="main-img" />
      <h3>Kit Fitness y Salud</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/YWY_9y05HBU" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Complementa tu rutina deportiva y mejora tu bienestar físico.
      </div>
    </div>

    <!-- Kit 6: Belleza y Relajación -->
    <div class="kit">
      <img src="https://i.imgur.com/Vk3RsVp.jpg" alt="Belleza y Relajación" class="main-img" />
      <h3>Kit Belleza y Relajación</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/VvqvDKRbgvY" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Ideal para desconectar, relajarse y cuidar cuerpo y mente desde casa.
      </div>
    </div>

  </div> <!-- Cierra .kits-container -->

  <footer>
    <p>Contacto: +51 934 172 944</p>
    <div class="social-icons">
      <a href="https://www.instagram.com/femmebox_oficial?igsh=MXQyc2VxN3dpdmkzYQ==" target="_blank">
        <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAABx0lEQVRYR+2XzUoDQRSG/0mcP4eG4BNH4I+hCbzA0sQs5ALuBvgg+AoZMg8gwkexkENIBEl0QJgskfUlF5hVq1d79t7/LeZ5hFvJr9T1TQwnqgW5wevV+41APQGkB18BqwmVDBxH77VtZ7kOYD9Q0xY5+oGqPQJ5AvYGUd9JG2iPPhXIfwe7gVwDbkuVoD3sP+Af4rHnN6iuZpWtImGblfQHb4C5yeff0v7L+uCL6QvZLoPnQBtU6pJ7C5jIO8AB6E8iAh4B7wDs3A+cLZyBHOwBfgC3kO8Ar+0pYaY4SIlXwwAfQZzDwrEN7Aq93IqgmxD/XA+uA9tElGJ0Db8qD3K53/ChbRJaYH+gcf7oJY8Z2gRuzF/gbnX8Gryi2ECg+ewBd6iTRwB7KKdwD3wDo6I5hI12lWDRSWhLq0ng2XYRr8p63m9mnfS+5vx8wrtKkH/ZPEHYOkxXAAAAAElFTkSuQmCC" alt="Instagram" />
      </a>
      <a href="https://wa.me/51934172944" target="_blank">
        <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAABd0lEQVRYR+2WQQrCQBBFv+sl9Ax0AvyKq6IgCCdo0QAUUgBM6Eg3Q8vUFxU3UjGPns+82fJf2xjS91hFOELg3HcY4x93GAGlBj0AdB+Mbkz0AzgMc4K1AzgN7AfkMJxF5gBhXauK8NpoQ7g+eTgJZBv1pVYw2s6IQG7BHOw8a6B9YFfw0bVwA9kCH4cZ2BJGB5ht7Ayzh+XB+QqZkxvwA0A6yj9QFFcCz8BZwBLv9Rm3jBSwCu0HnQ0kLncK6Q78wGA+j+XYk0H0MxFA7QdJxIB5x10Upt+AvUjmu4sjcPhQAAAABJRU5ErkJggg==" alt="WhatsApp" />
      </a>
    </div>
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



