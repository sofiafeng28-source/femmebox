<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>FemmeBox</title>
<style>
body{font-family:Arial,sans-serif;margin:0;padding:0;background:linear-gradient(135deg,#ffe9f3,#ffe0fb);}
header{padding:20px;text-align:center;background:#ff4081;color:#fff;}
.section-container{background:#fff;margin:20px auto;max-width:900px;border-radius:15px;padding:20px;box-shadow:0 4px 10px rgba(0,0,0,0.1);}
.kits-container{display:flex;flex-wrap:wrap;justify-content:center;padding:20px;gap:20px;}
.kit{background:#fff;border-radius:15px;width:300px;box-shadow:0 4px 10px rgba(0,0,0,0.1);text-align:center;padding:15px;display:flex;flex-direction:column;align-items:center;}
.kit img{width:140px;height:140px;border-radius:50%;object-fit:cover;}
.kit h3{color:#ff4081;margin:10px 0;}
.kit p{font-size:14px;color:#555;}
.kit button{background:#ff4081;color:#fff;border:none;padding:10px;border-radius:5px;cursor:pointer;margin-top:10px;}
.kit button:hover{background:#e040fb;}
.extra-content{display:none;text-align:left;margin-top:10px;font-size:13px;color:#555;}
iframe{width:100%;height:160px;border:none;border-radius:10px;margin-top:10px;}
.integrantes-container{display:flex;flex-wrap:wrap;justify-content:center;gap:20px;}
.integrante{text-align:center;}
.integrante img{width:120px;height:120px;border-radius:50%;object-fit:cover;}
footer{background:#ff4081;color:#fff;text-align:center;padding:20px;}
footer .social-icons{margin-top:10px;}
footer .social-icons a{margin:0 10px;}
footer .social-icons img{width:35px;height:35px;border-radius:50%;object-fit:cover;}
</style>
</head>
<body>

<header>
<h1>FemmeBox - Kits de Bienestar</h1>
</header>

<!-- Quiénes Somos -->
<section class="section-container">
<h2 style="color:#ff4081;text-align:center;">Quiénes Somos</h2>
<p style="text-align:center;color:#555;font-size:14px;">FemmeBox es un proyecto dedicado a crear kits de bienestar personalizados para diferentes etapas de la vida, promoviendo autocuidado, salud y equilibrio emocional.</p>
</section>

<!-- Kits -->
<div class="kits-container">

<div class="kit">
<img src="https://i.imgur.com/a/g5PqA2Z/1.jpg" alt="Bienestar Juvenil" loading="lazy">
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

<!-- Repetir para los demás kits... usando loading="lazy" en img e iframe -->

</div>

<!-- Integrantes -->
<section class="section-container">
<h2 style="color:#ff4081;text-align:center;">Integrantes</h2>
<div class="integrantes-container">
<div class="integrante">
<img src="https://i.imgur.com/a/g5PqA2Z/12.jpg" alt="Integrante 1" loading="lazy">
<p style="color:#555;font-size:14px;">Nombre 1</p>
</div>
<div class="integrante">
<img src="https://i.imgur.com/a/g5PqA2Z/13.jpg" alt="Integrante 2" loading="lazy">
<p style="color:#555;font-size:14px;">Nombre 2</p>
</div>
<div class="integrante">
<img src="https://i.imgur.com/a/g5PqA2Z/14.jpg" alt="Integrante 3" loading="lazy">
<p style="color:#555;font-size:14px;">Nombre 3</p>
</div>
</div>
</section>

<footer>
<p>Contacto: +51 934 172 944</p>
<div class="social-icons">
<a href="https://www.instagram.com/femmebox_oficial" target="_blank">
<img src="https://i.imgur.com/a/g5PqA2Z/10.jpg" alt="Instagram" loading="lazy">
</a>
<a href="https://wa.me/51934172944" target="_blank">
<img src="https://i.imgur.com/a/g5PqA2Z/11.jpg" alt="WhatsApp" loading="lazy">
</a>
</div>
</footer>

<script>
function toggleContent(button){
const content=button.nextElementSibling;
if(content.style.display==="block"){content.style.display="none";button.textContent="Ver más";}
else{content.style.display="block";button.textContent="Ver menos";}
}
</script>

</body>
</html>

