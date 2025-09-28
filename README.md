<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>FemmeBox</title>
<style>
* { box-sizing: border-box; margin:0; padding:0; font-family: Arial,sans-serif; text-align:center;}
body { background: linear-gradient(135deg,#ffe9f3,#ffe0fb); padding:40px 20px;}
header { font-size:2.5rem; color:#d81b60; margin-bottom:40px;}
.kits-container { display:flex; flex-wrap:wrap; justify-content:center; gap:40px;}
.kit { background:white; border-radius:25px; width:350px; padding:25px; box-shadow:0 15px 35px rgba(216,27,96,0.15);}
.kit img { width:140px; height:140px; border-radius:50%; object-fit:cover; margin-bottom:15px;}
.video-container { margin:15px 0; border-radius:15px; overflow:hidden; }
.video-container iframe { width:100%; height:180px; border:none;}
.info-text { font-size:0.9rem; margin-bottom:15px;}
.ver-mas { display:inline-block; background:linear-gradient(135deg,#d81b60,#f48fb1); color:white; padding:10px 20px; border-radius:30px; cursor:pointer; border:none; margin-bottom:10px;}
.ver-mas:hover { background:linear-gradient(135deg,#f48fb1,#d81b60);}
.extra-content { max-height:0; overflow:hidden; transition:max-height 0.5s ease; text-align:left; font-size:0.9rem; margin-top:10px;}
.extra-content ol { padding-left:20px; }
footer { margin-top:40px; padding:20px 0; background:#f8bbd0; color:white; border-radius:20px 20px 0 0;}
.social-icons { margin-top:10px;}
.social-icons a { margin:0 10px; display:inline-block;}
.social-icons img { width:38px; height:38px; object-fit:contain;}
</style>
</head>
<body>

<header>FemmeBox - Kits de Bienestar</header>

<div class="kits-container">

<!-- Kit Adolescencia -->
<div class="kit">
  <img src="https://i.imgur.com/ze21zby.jpg" alt="Adolescencia">
  <h3>Kit Bienestar Juvenil</h3>
  <div class="video-container">
    <iframe src="https://www.youtube.com/embed/dZiJp76DLe4" allowfullscreen></iframe>
  </div>
  <div class="info-text">Productos esenciales para jóvenes que comienzan a cuidar su cuerpo y bienestar de forma responsable.</div>
  <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ol>
      <li>Gel facial suave</li>
      <li>Desodorante natural</li>
      <li>Toallitas húmedas reutilizables</li>
      <li>Agenda de autocuidado</li>
      <li>Mini espejo portátil</li>
      <li>Estuche organizador</li>
    </ol>
  </div>
</div>

<!-- Kit Cuidado de piel -->
<div class="kit">
  <img src="https://i.imgur.com/MfODBjN.jpg" alt="Cuidado de piel">
  <h3>Kit Cuidado de Piel</h3>
  <div class="video-container">
    <iframe src="https://www.youtube.com/embed/eKjIgG0xuU8" allowfullscreen></iframe>
  </div>
  <div class="info-text">Mantén tu piel sana y radiante con productos específicos según tu tipo de piel.</div>
  <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ol>
      <li>Limpiador facial</li>
      <li>Tónico equilibrante</li>
      <li>Crema hidratante</li>
      <li>Protector solar</li>
      <li>Mascarilla facial</li>
      <li>Bolsa organizadora</li>
    </ol>
  </div>
</div>

<!-- Kit Postparto -->
<div class="kit">
  <img src="https://i.imgur.com/n1LFtB6.jpg" alt="Postparto">
  <h3>Kit Postparto</h3>
  <div class="video-container">
    <iframe src="https://www.youtube.com/embed/UpGV7QXKzPI" allowfullscreen></iframe>
  </div>
  <div class="info-text">Soporte esencial para las mamás durante la recuperación y adaptación tras el nacimiento.</div>
  <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ol>
      <li>Crema anti-estrías</li>
      <li>Cojín de lactancia</li>
      <li>Ropa cómoda postparto</li>
      <li>Toallitas y pañales</li>
      <li>Guía de cuidados</li>
      <li>Bolsa de maternidad</li>
    </ol>
  </div>
</div>

<!-- Kit Bienestar Emocional -->
<div class="kit">
  <img src="https://i.imgur.com/NUegUh8.jpg" alt="Bienestar Emocional">
  <h3>Kit Bienestar Emocional</h3>
  <div class="video-container">
    <iframe src="https://www.youtube.com/embed/LWeWviJJHoo" allowfullscreen></iframe>
  </div>
  <div class="info-text">Fortalece el amor propio y la salud emocional con productos prácticos.</div>
  <button class="ver-mas" onclick="toggleContent(this)">Ver más</button>
  <div class="extra-content">
    <ol>
      <li>Cuaderno de gratitud</li>
      <li>Té relajante</li>
      <li>Difusor portátil</li>
      <li>Tarjetas motivacionales</li>
      <li>Goma antiestrés</li>
      <li>Bolso organizador</li>
    </ol>
  </div>
</div>

</div> <!-- cierre kits-container -->

<footer>
  <p>Contacto: +51 934 172 944</p>
  <div class="social-icons">
    <a href="https://www.instagram.com/femmebox_oficial?igsh=MXQyc2VxN3dpdmkzYQ==" target="_blank">
      <img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" alt="Instagram">
    </a>
    <a href="https://wa.me/51934172944" target="_blank">
      <img src="https://upload.wikimedia.org/wikipedia/commons/5/5e/WhatsApp_icon.png" alt="WhatsApp">
    </a>
  </div>
</footer>

<script>
function toggleContent(button){
  const content = button.nextElementSibling;
  if(content.style.maxHeight){
    content.style.maxHeight = null;
    button.textContent = "Ver más";
  }else{
    content.style.maxHeight = content.scrollHeight + "px";
    button.textContent = "Ver menos";
  }
}
</script>

</body>
</html>


