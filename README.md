# BootcampMedTechFest
Código de página de lanzamiento

HTML

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Santiago Mazo</title>
  <link rel="stylesheet" href="css/styles.css">
  <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.15.4/css/all.css" integrity="sha384-DyZ88mC6Up2uqS4h/KRgHuoeGwBcD4Ng9SiP4dIRy0EXTlnuz47vAwmeGwVChigm" crossorigin="anonymous">
</head>
<body>

  <div class="wrapper">
    <header>
      <nav class="navbar">
        <div class="brand">
          <h2>S<span>M</span></h2>
        </div>
      <ul class="menu">
        <li><a class="active" href="#">Inicio</a></li>
        <li><a href="#">Sobre mí</a></li>
        <li><a href="#">Portafolio</a></li>
        <li><a href="#">Contacto</a></li>
      </ul>
       </nav>
    </header>
    <main class="main">
      <div class= "info-content" >
        <h1>Yo soy <span>Santiago</span> Mazo</h1>
        <p>Profesional en Negocios Internacionales con estudios adicionales en gestión de proyectos y experiencia en marketing digital y comercio electrónico. Mi propósito es generar o hacer parte de emprendimientos de alto impacto social y ambiental que a través de herramientas de base tecnológica transformen la vida de las personas.</p>
        <a download href="#">
          <button class="download-cv">Descarga mi CV</button>
        </a>
      </div>
      <img src="C:\Users\USUARIO\Documents\portfolio-tutorial-master\img\pexels-photo-1516680-removebg-preview.png" alt="Foto Santiago"> 
    </main>
  </div>

    <div class="about">
      <img src="img/about.png" alt= "Retrato Santiago">

      <div class="about-info">
        <h2>Sobre mí</h2>
        <div class="divider"></div>
        <p>Lorem ipsum hshhshdhdbfydfbdyfbdyfysdufyusdfysufusfuys</p>
        <p>Lorem ipsum hshhshdhdbfydfbdyfbdyfysdufyusdfysufusfuys</p>
        <butoom class="download-cv">Leer más</butoom>
    
      </div>
    </div>
  
  <div class="portfolio">
    <div class="portfolio-headings">
      <h2>Mi portafolio</h2>
      <div class="divider"></div>
    </div>

    <div class="container">
      <div class="card">
        <div class="card_img">
        </div>
        <div class="card_title">
          <h2>Descripción del servicio</h2>
          <p>Lorem ipsum y otras cosas más sobre el servicio</p>
        </div>
        <div class="projects-links">
          <a href="">
            <i class="fa-brands fa-github"></i>
          </a>
          <a href="">
            <i class="fa-solid fa-earth-americas"></i>
          </a>
          <a href="">
            <i class="fa-solid fa-code"></i>
          </a>
        </div>
        <div class="project-details-content">
         <button class="project-details download-cv">
          <a href="">
            Descripción del servicio
          </a>
        </button>  
        </div>
      </div>
    </div>
  </div>

</body>
</html>

CSS

@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;700&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Montserrat', sans-serif;
  overflow-x: hidden;
}

.wrapper {
  width: 100vw;
  height: 100vh;
  background-color: #191c32;
  color: #fff
}

.navbar {
display: flex;
justify-content: space-between;
padding: 2em;
}

.brand {
  margin-top: -7px;
}

.brand span{
  color:aqua;
}

.menu {
  display:flex;
  width: 50%;
  justify-content: space-around;
}
.menu li{
  list-style: none;
}
.menu a {
  color: #fff;
  text-decoration: none;
  padding: 10px 20px;
}

.menu .active {
  color:aqua
}

.menu a:hover {
  background-color: aqua;
  color: #191c32;
}

.main {
  margin: 0 auto;
  width: 80vw;
  height: 80vh;
  display: grid;
  grid-template-columns: repeat(2,1fr);
  align-items: center;
}

h1 {
  font-size: 3em;
}

span {
  color: aqua
}

.download-cv {
  padding: 10px 20px ;
  background-color: aqua;
  border: none;
  border-radius: 20px;
  margin-top: 10px;
  cursor: pointer;
  box-shadow: 1px 3px 11px -5px rgba(102, 231, 200, 0.69);
}

.download-cv:hover {
  background-color: #fff ;
  box-shadow: none;
}

.main img {
   width: 350px;
   border: 7px solid aqua;
   height: 520px;
   margin-left: 5em;
}

.about {
  display: grid;
  grid-template-columns: repeat(10, 1fr);
  width: 100vw;
  align-items: center;
}

.about img {
  width:100%;
  grid-column: 1/5;
}

.about-info {
  grid-column: 5/10;
  padding: 3em;
}

.about-info h2 {
  font-size: 2em;
  color: #191c32
}

.divider {
  height: 4px;
  width: 68px;
  background-color: aqua;
  margin-top: 3px;
  margin-bottom: 1em;
}

.about p {
  margin-bottom: 1.5em;
}

.portfolio {
 width: 100vw;
 background-color: #191c32;
 color:#fff;
}

.portfolio-headings {
  width: 100vw;
  padding:5em;
}

.portfolio-headings h2 {
  font-size: 2.5em;
}

.portfolio .container {
  width: 80vw;
  height: 80vh;
  margin: 0 auto;
  display: flex;
  justify-content: center;
}

.card {
  width: 300px;
  height: 350px;
  color: #fff;
  background-color: #101e4b;
}

.card_img {
  width: 100%;
  height: 150px;
  background-image: url(../img/2-original.png);
  background-size: cover;
}

.card_title {
  padding: 20px;
}

.card_project-links {
  display: flex;
  justify-content: space-evenly;
}

.card_project-links a {
  color: #fff;
  text-decoration: none ;
}

.card_project-links i {
  font-size: 1.5em;
} 

.card .project-details {
  margin: 0 auto;
  margin: 1em;
  width: 70%;
} 

.card .project-details a {
  text-decoration: none;
  color: #191c32;
  text-transform: uppercase;
}

.project-details-content {
  display: flex;
  width: 100%;
  justify-content: center;
  margin-top: 1em;
}
