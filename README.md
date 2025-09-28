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

    <!-- Kit 1 Original -->
    <div class="kit">
      <img src="https://i.imgur.com/rbGqFUv.jpg" alt="Primera menstruación" class="main-img" />
      <h3>Kit Primera Menstruación</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/3hBqSbR5lF4" title="Video sobre la menstruación" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        La menstruación es un proceso natural en la vida de toda mujer. Aquí aprenderás sobre higiene y cuidados durante el ciclo menstrual para sentirte cómoda y segura.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit Primera Menstruación:</p>
        <ol class="products-list">
          <li>Panty liners o protectores diarios suaves</li>
          <li>Copa menstrual o toallas femeninas ecológicas</li>
          <li>Jabón íntimo neutro para piel sensible</li>
          <li>Crema calmante para la irritación</li>
          <li>Libro o guía educativa sobre menstruación</li>
          <li>Bolsa de tela reutilizable para transportar los productos</li>
        </ol>
        <div class="testimonials">
          "Sentí que por fin había un kit hecho para mí, con todo lo que necesito para sentirme segura y apoyada." - Ana G.
        </div>
      </div>
    </div>

    <!-- Kit 2 Original -->
    <div class="kit">
      <img src="https://i.imgur.com/TsgMJVj.jpg" alt="Kit Mamás" class="main-img" />
      <h3>Kit para Mamás</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/BM_2RDi9i7Yy" title="Video sobre embarazo" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Información esencial sobre el embarazo y cuidados que toda mamá debe conocer para una experiencia saludable y feliz.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit para Mamás:</p>
        <ol class="products-list">
          <li>Vitaminas prenatales y suplementos nutricionales</li>
          <li>Crema anti-estrías y cosméticos naturales</li>
          <li>Cojín de lactancia y almohada de soporte</li>
          <li>Libros sobre embarazo y maternidad</li>
          <li>Ropa cómoda para el postparto</li>
          <li>Bolsa de maternidad con artículos esenciales</li>
        </ol>
        <div class="testimonials">
          "Este kit me ayudó a sentirme apoyada y cuidada durante todo mi embarazo." - María L.
        </div>
      </div>
    </div>

    <!-- Kit 3 Original -->
    <div class="kit">
      <img src="https://i.imgur.com/Y8Zl6Dn.jpg" alt="Menopausia" class="main-img" />
      <h3>Kit Menopausia</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/EI9j0QzywuA" title="Video sobre menopausia" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        La menopausia es una etapa natural en la vida de toda mujer. Aprende por qué es normal y cómo cuidarte para mantener una buena calidad de vida.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit Menopausia:</p>
        <ol class="products-list">
          <li>Suplementos para el equilibrio hormonal</li>
          <li>Cremas hidratantes específicas para piel madura</li>
          <li>Productos para el alivio de bochornos</li>
          <li>Libros y guías sobre salud en menopausia</li>
          <li>Accesorios para ejercicio y relajación</li>
          <li>Infusiones naturales calmantes</li>
        </ol>
        <div class="testimonials">
          "Me encanta este kit porque me hace sentir que no estoy sola en esta etapa de cambio." - Laura M.
        </div>
      </div>
    </div>
    <!-- Kit 4 Nuevo -->
    <div class="kit">
      <img src="https://i.imgur.com/ze21zby.jpg" alt="Kit 4" class="main-img" />
      <h3>Kit de Bienestar Juvenil</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/VIDEO_ID_1" title="Video sobre bienestar juvenil" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Productos esenciales para jóvenes que comienzan a cuidar su cuerpo y bienestar de forma responsable.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit:</p>
        <ol class="products-list">
          <li>Gel facial suave</li>
          <li>Desodorante natural</li>
          <li>Toallitas húmedas reutilizables</li>
          <li>Agenda de autocuidado</li>
          <li>Mini espejo portátil</li>
          <li>Estuche organizador</li>
        </ol>
        <div class="testimonials">
          "Ideal para comenzar a cuidarme con productos adecuados a mi edad." - Camila R.
        </div>
      </div>
    </div>

    <!-- Kit 5 Nuevo -->
    <div class="kit">
      <img src="https://i.imgur.com/NUegUh8.jpg" alt="Kit 5" class="main-img" />
      <h3>Kit Autoestima y Cuidado Personal</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/VIDEO_ID_2" title="Video sobre autoestima" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Pensado para fortalecer el amor propio y el bienestar emocional con productos prácticos.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit:</p>
        <ol class="products-list">
          <li>Libreta de afirmaciones positivas</li>
          <li>Crema hidratante corporal</li>
          <li>Velas aromáticas</li>
          <li>Mascarilla facial</li>
          <li>Infusiones relajantes</li>
          <li>Bolsa ecológica</li>
        </ol>
        <div class="testimonials">
          "Me ayudó a sentirme mejor conmigo misma y cuidar mi mente." - Sofía L.
        </div>
      </div>
    </div>

    <!-- Kit 6 Nuevo -->
    <div class="kit">
      <img src="https://i.imgur.com/Vk3RsVp.jpg" alt="Kit 6" class="main-img" />
      <h3>Kit Salud Deportiva</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/VIDEO_ID_3" title="Video sobre salud deportiva" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Ideal para mujeres activas que desean complementar su rutina con productos de bienestar físico.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit:</p>
        <ol class="products-list">
          <li>Botella reutilizable</li>
          <li>Toalla deportiva</li>
          <li>Proteína en polvo</li>
          <li>Gomas de resistencia</li>
          <li>Bálsamo para músculos</li>
          <li>Planner de ejercicios</li>
        </ol>
        <div class="testimonials">
          "Perfecto para complementar mi estilo de vida." - Fernanda S.
        </div>
      </div>
    </div>
    <!-- Kit 7 Nuevo -->
    <div class="kit">
      <img src="https://i.imgur.com/BGlMJPw.jpg" alt="Kit 7" class="main-img" />
      <h3>Kit Relajación y Spa</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/VIDEO_ID_4" title="Video sobre relajación" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Un kit pensado para desconectar, relajarse y cuidar cuerpo y mente desde casa.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit:</p>
        <ol class="products-list">
          <li>Sales de baño</li>
          <li>Mascarilla hidratante</li>
          <li>Aceite esencial</li>
          <li>Antifaz de descanso</li>
          <li>Exfoliante suave</li>
          <li>Esponja corporal</li>
        </ol>
        <div class="testimonials">
          "Una experiencia relajante sin salir de casa." - Valeria R.
        </div>
      </div>
    </div>

    <!-- Kit 8 Nuevo -->
    <div class="kit">
      <img src="https://i.imgur.com/n1LFtB6.jpg" alt="Kit 8" class="main-img" />
      <h3>Kit Salud Mental y Equilibrio</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/VIDEO_ID_5" title="Video sobre salud mental" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Diseñado para fomentar el bienestar emocional y la gestión del estrés.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit:</p>
        <ol class="products-list">
          <li>Cuaderno de gratitud</li>
          <li>Té relajante</li>
          <li>Difusor portátil</li>
          <li>Tarjetas motivacionales</li>
          <li>Goma antiestrés</li>
          <li>Bolso organizador</li>
        </ol>
        <div class="testimonials">
          "Me ayudó mucho en días de estrés." - Daniela M.
        </div>
      </div>
    </div>

    <!-- Kit 9 Nuevo -->
    <div class="kit">
      <img src="https://i.imgur.com/MfODBjN.jpg" alt="Kit 9" class="main-img" />
      <h3>Kit Cuidado Nocturno</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/VIDEO_ID_6" title="Video sobre cuidado nocturno" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Pensado para crear rutinas tranquilas antes de dormir y mejorar el descanso.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit:</p>
        <ol class="products-list">
          <li>Crema facial de noche</li>
          <li>Spray para almohada</li>
          <li>Pijama ligera</li>
          <li>Calcetas suaves</li>
          <li>Infusión para dormir</li>
          <li>Libro de relajación</li>
        </ol>
        <div class="testimonials">
          "Mi rutina nocturna cambió por completo." - Regina P.
        </div>
      </div>
    </div>

  </div> <!-- Cierra .kits-container -->

  <footer>
    <p>&copy; 2024 Tu Proyecto. Todos los derechos reservados.</p>
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

