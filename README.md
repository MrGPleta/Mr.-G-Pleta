# Mr.-G-Pleta
/index.html
/assets/
  ├─ css/
  │   └─ styles.css
  ├─ js/
  │   └─ main.js
  └─ images/
      ├─ hero-tripleta.jpg
      ├─ tripleta1.webp
      └─ ...  
<!DOCTYPE html>
<html lang="es" class="no-js">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Mr. G-Pleta – Puerto Rican Tripletas</title>
  <meta name="description" content="Disfruta la auténtica comida puertorriqueña en Mr. G-Pleta. Tripletas, catering y más.">
  <!-- Preconnect & Preload -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preload" href="assets/images/hero-tripleta.jpg" as="image">
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@600&family=Open+Sans&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="assets/css/styles.css">
</head>
<body>
  <header role="banner">
    <nav role="navigation" aria-label="Menú principal" class="navbar">
      <a href="#" class="logo">Mr. G-Pleta</a>
      <button id="menu-toggle" aria-expanded="false" aria-controls="nav-menu">☰</button>
      <ul id="nav-menu" class="nav-links">
        <li><a href="#home">Inicio</a></li>
        <li><a href="#menu">Menú</a></li>
        <li><a href="#gallery">Galería</a></li>
        <li><a href="#contact">Contacto</a></li>
      </ul>
    </nav>
    <div id="home" class="hero" role="region" aria-label="Sección de bienvenida">
      <img src="assets/images/hero-tripleta.jpg"
           alt="Tripleta puertorriqueña con carne, jamón y queso"
           loading="lazy" width="1200" height="800">
      <div class="hero-text">
        <h1>¡Bienvenidos a Mr. G-Pleta!</h1>
        <a href="#menu" class="button">Ver Menú</a>
      </div>
    </div>
  </header>

  <main role="main">
    <!-- Menu Section -->
    <section id="menu" role="region" aria-labelledby="menu-heading" class="section">
      <h2 id="menu-heading">Nuestro Menú</h2>
      <div class="menu-grid">
        <!-- Example Item -->
        <article class="menu-item">
          <picture>
            <source srcset="assets/images/tripleta1.webp" type="image/webp">
            <img src="assets/images/tripleta1.jpg"
                 alt="Tripleta clásica con carne frita"
                 loading="lazy" width="400" height="300">
          </picture>
          <h3>Tripleta Clásica</h3>
          <p>Carnes mixtas, queso amarillo y nuestro pan especial.</p>
          <a href="#contact" class="button small">Ordenar</a>
        </article>
        <!-- Add more items similarly -->
      </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery" role="region" aria-labelledby="gallery-heading" class="section">
      <h2 id="gallery-heading">Galería</h2>
      <div class="gallery-grid">
        <img src="assets/images/tripleta2.webp" alt="Tripleta con tostones" loading="lazy" width="400" height="300">
        <img src="assets/images/tripleta3.webp" alt="Tripleta con salsa" loading="lazy" width="400" height="300">
        <!-- More images -->
      </div>
    </section>

    <!-- Social Section -->
    <section id="social" role="region" aria-labelledby="social-heading" class="section">
      <h2 id="social-heading">Síguenos</h2>
      <!-- Instagram Embed -->
      <div class="embed">
        <blockquote class="instagram-media"
                    data-instgrm-permalink="https://www.instagram.com/p/CG0UU3HnF7p/"
                    data-instgrm-version="14">
        </blockquote>
        <script async defer src="//www.instagram.com/embed.js"></script> :contentReference[oaicite:4]{index=4}
      </div>
      <!-- TikTok Embed -->
      <div class="embed">
        <blockquote class="tiktok-embed"
                    cite="https://www.tiktok.com/@mr.g.pleta/video/6951234567890123457"
                    data-video-id="6951234567890123457"
                    style="max-width: 605px;min-width: 325px;">
        </blockquote>
        <script async src="https://www.tiktok.com/embed.js"></script> :contentReference[oaicite:5]{index=5}
      </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" role="region" aria-labelledby="contact-heading" class="section">
      <h2 id="contact-heading">Contacto</h2>
      <p>Ubicación actual del camión: <a href="https://goo.gl/maps/XYZ" target="_blank">Ver en Google Maps</a></p>
      <form aria-label="Formulario de reserva/catering">
        <label for="name">Nombre:</label>
        <input type="text" id="name" name="name" required>
        <label for="email">Correo:</label>
        <input type="email" id="email" name="email" required>
        <label for="message">Mensaje:</label>
        <textarea id="message" name="message" rows="4"></textarea>
        <button type="submit" class="button">Enviar</button>
      </form>
    </section>
  </main>

  <footer role="contentinfo" class="footer">
    <p>&copy; 2025 Mr. G-Pleta. Todos los derechos reservados.</p>
  </footer>

  <script src="assets/js/main.js"></script>
</body>
</html>
:root {
  --pr-red: #e30b17;
  --pr-blue: #0039a6;
  --pr-white: #ffffff;
  --font-heading: 'Montserrat', sans-serif;
  --font-body: 'Open Sans', sans-serif;
}

/* Reset & Base */
* { margin:0; padding:0; box-sizing:border-box; }
body {
  font-family: var(--font-body);
  line-height: 1.6;
  background: var(--pr-white);
  color: #333;
}

/* Typography & Contrast */
h1, h2, h3 { font-family: var(--font-heading); color: var(--pr-red); }
p, label { color: #111; }
a, .button { color: var(--pr-white); }

/* Navbar */
.navbar {
  background: var(--pr-blue);
  display: flex; align-items:center; justify-content:space-between;
  padding: 1rem;
  position: sticky; top:0; z-index:1000;
}
.logo { font-size:1.5rem; font-weight:bold; color: var(--pr-white); }
#menu-toggle { background:none; border:none; color: var(--pr-white); font-size:1.5rem; cursor:pointer; }
.nav-links { list-style:none; display:flex; gap:1rem; }
.nav-links li a { text-decoration:none; padding:0.5rem; }
@media (max-width:768px) {
  .nav-links { display:none; flex-direction:column; background: var(--pr-blue); width:100%; }
  .nav-links.show { display:flex; }
}

/* Hero */
.hero {
  position: relative; text-align:center; color: var(--pr-white);
}
.hero img { width:100%; height:auto; }
.hero-text {
  position:absolute; top:50%; left:50%; transform: translate(-50%, -50%);
}

/* Buttons */
.button {
  display:inline-block; background: var(--pr-red); padding:0.75rem 1.5rem;
  border-radius:0.5rem; text-decoration:none; transition:transform .2s ease;
}
.button:hover, .button:focus { transform: scale(1.05); }

/* Sections */
.section { padding:4rem 1rem; max-width:1200px; margin:0 auto; }
.menu-grid, .gallery-grid {
  display: grid; gap:1.5rem;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
}
.menu-item, .gallery-grid img { border-radius:0.5rem; overflow:hidden; }

/* Form */
form { display:grid; gap:1rem; max-width:600px; margin:2rem auto; }
input, textarea { width:100%; padding:0.75rem; border:1px solid #ccc; border-radius:0.25rem; }

/* Footer */
.footer { background:#222; color:#aaa; text-align:center; padding:1rem; }
// Toggle mobile menu
const toggle = document.getElementById('menu-toggle');
const menu  = document.getElementById('nav-menu');
toggle.addEventListener('click', () => {
  const expanded = toggle.getAttribute('aria-expanded') === 'true';
  toggle.setAttribute('aria-expanded', !expanded);
  menu.classList.toggle('show');
});
