<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FemmeBox</title>
<style>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background: linear-gradient(135deg, #ffe9f3, #ffe0fb);
}
header {
  text-align: center;
  padding: 20px;
  background-color: #ff4081;
  color: white;
}
.section-container {
  background:white; 
  margin:20px auto; 
  max-width:900px; 
  border-radius:15px; 
  padding:20px; 
  box-shadow:0 4px 10px rgba(0,0,0,0.1);
}
.kits-container {
  display:flex;
  flex-wrap:wrap;
  justify-content:center;
  padding:20px;
  gap:20px;
}
.kit {
  background:#fff;
  border-radius:15px;
  width:300px;
  box-shadow:0 4px 10px rgba(0,0,0,0.1);
  text-align:center;
  padding:15px;
  display:flex;
  flex-direction:column;
  align-items:center;
}
.kit img {
  width:200px;
  height:200px;
  border-radius:15px;
  object-fit:cover;
}
.kit h3 {
  color:#ff4081;
  margin:10px 0;
}
.kit p {
  font-size:14px;
  color:#555;
}
.kit button {
  background:#ff4081;
  color:#fff;
  border:none;
  padding:10px;
  border-radius:5px;
  cursor:pointer;
  margin-top:10px;
}
.kit button:hover {
  background:#e040fb;
}
.extra-content {
  display:none;
  text-align:left;
  margin-top:10px;
  font-size:13px;
  color:#555;
}
iframe {
  width:100%;
  height:160px;
  border:none;
  border-radius:10px;
  margin-top:10px;
}
.integrantes-container {
  display:flex;
  flex-direction:column;
  align-items:center;
  gap:15px;
}
footer {
  background:#ff4081;
  color:#fff;
  text-align:center;
  padding:20px;
}
footer .social-icons {
  margin-top:10px;
}
footer .social-icons a {
  margin:0 10px;
}
footer .social-icons img {
  width:35px;
  height:35px;
  border-radius:50%;
  object-fit:cover;
}
</style>
</head>
<body>

<header>
  <h1>FemmeBox - Kits de Bienestar</h1>
</header>

<!-- Quiénes Somos -->
<section class="section-container">
  <h2 style="color:#ff4081;text-align:center;">Quiénes Somos</h2>
  <p style="text-align:center;color:#555;font-size:14px;">
    FemmeBox es un proyecto dedicado a crear kits de bienestar personalizados para diferentes etapas de la vida, promoviendo autocuidado, salud y equilibrio emocional.
  </p>
</section>

<!-- Kits -->
<div class="kits-container">

<!-- Kit 1 -->
<div class="kit">
  <img src="https://i.imgur.com/ze21zby.jpg" alt="Bienestar Juvenil" loading="lazy">
  <h3>Kit Bienestar Juvenil</h3>
  <iframe loading="lazy" src="https://www.youtube.com/embed/dZiJp76DLe4" allowfullscreen></iframe>
  <p>Productos esenciales para jóvenes que comienzan a cuidar su cuerpo y bienestar.</p>
  <button onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ul>
      <li>Gel facial suave</li>
      <li>Desodorante natural</li>
      <li>Toallitas húmedas reutilizables</li>
      <li>Agenda de autocuidado</li>
      <li>Mini espejo portátil</li>
      <li>Estuche organizador</li>
    </ul>
  </div>
</div>

<!-- Kit 2 -->
<div class="kit">
  <img src="https://i.imgur.com/MfODBjN.jpg" alt="Cuidado de Piel" loading="lazy">
  <h3>Kit Cuidado de Piel</h3>
  <iframe loading="lazy" src="https://www.youtube.com/embed/eKjIgG0xuU8" allowfullscreen></iframe>
  <p>Productos para mantener la piel limpia, hidratada y saludable.</p>
  <button onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ul>
      <li>Limpiador facial</li>
      <li>Crema hidratante</li>
      <li>Protector solar</li>
      <li>Mascarilla facial</li>
      <li>Tónico refrescante</li>
    </ul>
  </div>
</div>

<!-- Kit 3 -->
<div class="kit">
  <img src="https://i.imgur.com/n1LFtB6.jpg" alt="Postparto" loading="lazy">
  <h3>Kit Postparto</h3>
  <iframe loading="lazy" src="https://www.youtube.com/embed/UpGV7QXKzPI" allowfullscreen></iframe>
  <p>Cuidados esenciales durante la etapa postparto.</p>
  <button onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ul>
      <li>Crema para estrías</li>
      <li>Almohada de soporte</li>
      <li>Ropa cómoda</li>
      <li>Libros sobre maternidad</li>
    </ul>
  </div>
</div>

<!-- Kit 4 -->
<div class="kit">
  <img src="https://i.imgur.com/NUegUh8.jpg" alt="Bienestar Emocional" loading="lazy">
  <h3>Kit Bienestar Emocional</h3>
  <iframe loading="lazy" src="https://www.youtube.com/embed/LWeWviJJHoo" allowfullscreen></iframe>
  <p>Fortalece el amor propio y el equilibrio emocional.</p>
  <button onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ul>
      <li>Cuaderno de gratitud</li>
      <li>Té relajante</li>
      <li>Tarjetas motivacionales</li>
      <li>Goma antiestrés</li>
    </ul>
  </div>
</div>

<!-- Kit 5 -->
<div class="kit">
  <img src="https://i.imgur.com/BGlMJPw.jpg" alt="Fitness y Salud" loading="lazy">
  <h3>Kit Fitness y Salud</h3>
  <iframe loading="lazy" src="https://www.youtube.com/embed/YWY_9y05HBU" allowfullscreen></iframe>
  <p>Complementa tu rutina deportiva y bienestar físico.</p>
  <button onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ul>
      <li>Botella reutilizable</li>
      <li>Toalla deportiva</li>
      <li>Proteína en polvo</li>
      <li>Gomas de resistencia</li>
      <li>Bálsamo para músculos</li>
    </ul>
  </div>
</div>

<!-- Kit 6 -->
<div class="kit">
  <img src="https://i.imgur.com/Vk3RsVp.jpg" alt="Belleza y Relajación" loading="lazy">
  <h3>Kit Belleza y Relajación</h3>
  <iframe loading="lazy" src="https://www.youtube.com/embed/VvqvDKRbgvY" allowfullscreen></iframe>
  <p>Productos para desconectar, relajarse y cuidar cuerpo y mente.</p>
  <button onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ul>
      <li>Mascarilla hidratante</li>
      <li>Sales de baño</li>
      <li>Aceite esencial</li>
      <li>Antifaz de descanso</li>
      <li>Exfoliante</li>
    </ul>
  </div>
</div>

<!-- Kit 7 -->
<div class="kit">
  <img src="https://i.imgur.com/TsgMJVj.jpg" alt="Kit Mamás" loading="lazy">
  <h3>Kit Mamás</h3>
  <iframe loading="lazy" src="https://www.youtube.com/embed/BM_2RDi9i7Yy" allowfullscreen></iframe>
  <p>Cuidados y productos para el embarazo y postparto.</p>
  <button onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ul>
      <li>Vitaminas prenatales</li>
      <li>Cojín de lactancia</li>
      <li>Ropa cómoda</li>
      <li>Libros sobre maternidad</li>
    </ul>
  </div>
</div>

<!-- Kit 8 -->
<div class="kit">
  <img src="https://i.imgur.com/Y8Zl6Dn.jpg" alt="Menopausia" loading="lazy">
  <h3>Kit Menopausia</h3>
  <iframe loading="lazy" src="https://www.youtube.com/embed/EI9j0QzywuA" allowfullscreen></iframe>
  <p>Cuidados para mantener la calidad de vida durante la menopausia.</p>
  <button onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ul>
      <li>Suplementos hormonales</li>
      <li>Cremas hidratantes</li>
      <li>Accesorios para ejercicio</li>
      <li>Infusiones naturales</li>
    </ul>
  </div>
</div>

<!-- Kit 9 -->
<div class="kit">
  <img src="https://i.imgur.com/MfODBjN.jpg" alt="Cuidado Nocturno" loading="lazy">
  <h3>Kit Cuidado Nocturno</h3>
  <iframe loading="lazy" src="https://www.youtube.com/embed/UpGV7QXKzPI" allowfullscreen></iframe>
  <p>Rutinas antes de dormir para mejorar descanso y relajación.</p>
  <button onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ul>
      <li>Crema facial de noche</li>
      <li>Spray para almohada</li>
      <li>Pijama ligera</li>
      <li>Infusión para dormir</li>
    </ul>
  </div>
</div>

</div>

<!-- Integrantes -->
<section class="section-container">
  <h2 style="color:#ff4081;text-align:center;">Integrantes</h2>
  <div class="integrantes-container">
    <div class="integrante">
      <p style="color:#555;font-size:14px;"><strong>Sofia Feng</strong><br>Diseñadora del prototipo (app y logotipo)</p>
    </div>
    <div class="integrante">
      <p style="color:#555;font-size:14px;"><strong>Piero Lopez</strong><br>Encargado de kits (armar ejemplos de productos)</p>
    </div>
    <div class="integrante">
      <p style="color:#555;font-size:14px;"><strong>Dhanna Rojas</strong><br>Marketing y comunicación (difusión en el colegio)</p>
    </div>
  </div>
</section>

<!-- Footer -->
<footer>
  <p>Contacto: +51 934 172 944</p>
  <div class="social-icons">
    <a href="https://www.instagram.com/femmebox_oficial" target="_blank">
      <img src="https://i.imgur.com/73Waibk.jpg" alt="Instagram" loading="lazy">
    </a>
    <a href="https://wa.me/51934172944" target="_blank">
      <img src="https://i.imgur.com/SdduDqI.jpg" alt="WhatsApp" loading="lazy">
    </a>
  </div>
</footer>

<script>
function toggleContent(button) {
  const content = button.nextElementSibling;
  if(content.style.display === "block") {
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




