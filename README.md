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
    .box {
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
    .integrantes-box h2,
    .quienes-somos h2 {
      color: #d81b60;
      margin-bottom: 15px;
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

  <section class="box quienes-somos">
    <h2>Quiénes somos</h2>
    <p>Ofrecemos kits personalizados de productos de cuidado y bienestar según la etapa de la vida de la mujer.</p>
    <p>Porque las mujeres suelen comprar productos de forma separada y sin orientación, lo que es costoso y poco práctico.</p>
    <p>Facilitamos el acceso a productos esenciales, promovemos el autocuidado femenino y brindamos información confiable de salud y bienestar.</p>
  </section>

  <section class="box integrantes-box">
    <h2>Integrantes</h2>
    <p><strong>Sofia Feng</strong> → Diseñadora del prototipo (app y logotipo).</p>
    <p><strong>Piero Lopez</strong> → Encargado de kits (armar ejemplos de productos).</p>
    <p><strong>Dhanna Rojas</strong> → Marketing y comunicación (difusión en el colegio).</p>
  </section>

  <div class="kits-container">

    <!-- KIT 1 ORIGINAL -->
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

    <!-- KIT 2 ORIGINAL -->
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

    <!-- KIT 3 ORIGINAL -->
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

    <!-- KIT 4 NUEVO -->
    <div class="kit">
      <img src="https://i.imgur.com/ze21zby.jpg" alt="Kit Adolescencia" class="main-img" />
      <h3>Kit Adolescencia y Autocuidado</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/DlgISiYDU7E" title="Autocuidado en adolescentes" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Acompaña los cambios físicos y emocionales de la adolescencia con productos y guía pensados para el bienestar femenino.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit Adolescencia y Autocuidado:</p>
        <ol class="products-list">
          <li>Desodorante natural</li>
          <li>Toallas higiénicas o copa reutilizable</li>
          <li>Gel limpiador facial suave</li>
          <li>Agenda o cuaderno de autocuidado</li>
          <li>Snacks saludables</li>
          <li>Bolsa reutilizable</li>
        </ol>
        <div class="testimonials">
          "Me ayudó a sentirme más preparada en una etapa llena de cambios." - Camila S.
        </div>
      </div>
    </div>

    <!-- KIT 5 NUEVO -->
    <div class="kit">
      <img src="https://i.imgur.com/NUegUh8.jpg" alt="Kit Cuidado Facial" class="main-img" />
      <h3>Kit Cuidado Facial y Piel</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/Rc2Qd2c12yk" title="Cuidado facial" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Ideal para mantener una piel limpia, hidratada y saludable con productos esenciales de uso diario.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit Cuidado Facial y Piel:</p>
        <ol class="products-list">
          <li>Limpiador facial suave</li>
          <li>Hidratante ligera</li>
          <li>Protector solar</li>
          <li>Mascarilla facial</li>
          <li>Toalla facial reutilizable</li>
          <li>Bolsa organizadora</li>
        </ol>
        <div class="testimonials">
          "Mi rutina se volvió más fácil y efectiva con este kit." - Paola R.
        </div>
      </div>
    </div>

    <!-- KIT 6 NUEVO -->
    <div class="kit">
      <img src="https://i.imgur.com/Vk3RsVp.jpg" alt="Kit Postparto" class="main-img" />
      <h3>Kit Postparto y Recuperación</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/itYgnPZXoqc" title="Recuperación postparto" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Pensado para ayudar a la mamá en los primeros meses tras el nacimiento del bebé, con productos de cuidado y bienestar.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit Postparto y Recuperación:</p>
        <ol class="products-list">
          <li>Faja postparto</li>
          <li>Crema reafirmante</li>
          <li>Compresas frías/calientes</li>
          <li>Snacks nutritivos</li>
          <li>Botella de agua reutilizable</li>
          <li>Bolsa organizadora</li>
        </ol>
        <div class="testimonials">
          "Me sentí cuidada y acompañada en la etapa más difícil." - Andrea F.
        </div>
      </div>
    </div>

    <!-- KIT 7 NUEVO -->
    <div class="kit">
      <img src="https://i.imgur.com/BGlMJPw.jpg" alt="Kit Bienestar Emocional" class="main-img" />
      <h3>Kit Bienestar Emocional</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/yW8sBEenNE4" title="Bienestar emocional" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Incluye herramientas para el autocuidado mental y manejo del estrés en la vida diaria.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit Bienestar Emocional:</p>
        <ol class="products-list">
          <li>Cuaderno de gratitud</li>
          <li>Infusiones relajantes</li>
          <li>Aceite esencial de relajación</li>
          <li>Tarjetas de afirmaciones</li>
          <li>Antifaz para descanso</li>
          <li>Bolsa de tela</li>
        </ol>
        <div class="testimonials">
          "Me ayudó a manejar mejor el estrés del día a día." - Fernanda M.
        </div>
      </div>
    </div>

    <!-- KIT 8 NUEVO -->
    <div class="kit">
      <img src="https://i.imgur.com/n1LFtB6.jpg" alt="Kit Fitness" class="main-img" />
      <h3>Kit Fitness y Salud Activa</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/1yH6Q4Z2IqY" title="Salud activa" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Perfecto para mujeres que buscan moverse, fortalecer su cuerpo y mantener hábitos saludables.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit Fitness y Salud Activa:</p>
        <ol class="products-list">
          <li>Bandas elásticas de ejercicio</li>
          <li>Botella deportiva</li>
          <li>Toalla absorbente</li>
          <li>Snacks proteicos</li>
          <li>Guía de estiramientos</li>
          <li>Bolsa deportiva</li>
        </ol>
        <div class="testimonials">
          "Me motivó a retomar el ejercicio con ganas." - Valeria T.
        </div>
      </div>
    </div>

    <!-- KIT 9 NUEVO -->
    <div class="kit">
      <img src="https://i.imgur.com/MfODBjN.jpg" alt="Kit Belleza" class="main-img" />
      <h3>Kit Belleza y Relajación</h3>
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/ol5U5ZsmuXw" title="Relajación" allowfullscreen></iframe>
      </div>
      <div class="info-text">
        Ideal para momentos de descanso, cuidado personal y spa en casa.
      </div>
      <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
      <div class="extra-content">
        <p>Contenido del Kit Belleza y Relajación:</p>
        <ol class="products-list">
          <li>Mascarillas faciales</li>
          <li>Sales de baño</li>
          <li>Velas aromáticas</li>
          <li>Crema hidratante</li>
          <li>Esponja exfoliante</li>
          <li>Bolsa de spa</li>
        </ol>
        <div class="testimonials">
          "Fue como tener un spa personal en casa." - Daniela P.
        </div>
      </div>
    </div>

  </div>

  <footer>
    <p>Contáctanos:</p>
    <div class="social-icons">
      <a href="https://wa.me/51934172944" target="_blank" rel="noopener noreferrer">
        <img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" alt="WhatsApp" />
      </a>
      <a href="https://www.instagram.com/femmebox_oficial?igsh=MXQyc2VxN3dpdmkzYQ==" target="_blank" rel="noopener noreferrer">
        <img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="Instagram" />
      </a>
    </div>
  </footer>

  <script>
    function toggleContent(button) {
      const extra = button.nextElementSibling;
      extra.classList.toggle('active');
      button.textContent = extra.classList.contains('active') ? 'Ver menos' : 'Ver más';
    }
  </script>

</body>
</html>

