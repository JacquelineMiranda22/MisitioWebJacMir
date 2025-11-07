<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Espacio Exterior — Recursos oficiales</title>
  <meta name="description" content="Sitio informativo sobre el espacio exterior con enlaces oficiales (NASA, ESA, SpaceX, ISRO), misiones y galería." />
  <style>
    :root{
      --bg:#05060a;
      --panel: rgba(255,255,255,0.04);
      --muted: #9aa4b2;
      --accent: #7dd3fc;
      --glass: linear-gradient(180deg, rgba(255,255,255,0.03), rgba(255,255,255,0.01));
      --radius: 14px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background: radial-gradient(1200px 600px at 10% 10%, rgba(15,23,42,0.6), transparent),
                  radial-gradient(1000px 500px at 90% 90%, rgba(2,6,23,0.6), transparent),
                  var(--bg);
      color:#e6eef8;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.45;
    }
    .container{max-width:1100px;margin:0 auto;padding:28px;}
    header{display:flex;align-items:center;justify-content:space-between;padding:14px 0}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{
      width:52px;height:52px;border-radius:12px;background:linear-gradient(135deg,#0ea5a4,#06b6d4);
      display:flex;align-items:center;justify-content:center;font-weight:700;color:#022;
      box-shadow: 0 6px 18px rgba(6,8,23,0.6);
    }
    nav a{color:var(--muted);text-decoration:none;margin-left:18px;font-weight:600}
    nav a:hover{color:var(--accent)}
    .hero{display:grid;grid-template-columns:1fr;gap:18px;align-items:center;padding:28px 0}
    @media(min-width:900px){ .hero{grid-template-columns:1fr 420px} }
    h1{font-size:32px;margin:0}
    .lead{color:var(--muted);margin-top:10px;font-size:16px}
    .card{background:var(--panel);padding:18px;border-radius:var(--radius);box-shadow: 0 6px 20px rgba(2,6,23,0.6);}
    .grid{display:grid;gap:14px}
    @media(min-width:700px){ .grid.cols-3{grid-template-columns:repeat(3,1fr)} .grid.cols-2{grid-template-columns:repeat(2,1fr)} }
    .muted{color:var(--muted);font-size:14px}
    .btn{display:inline-block;padding:9px 14px;border-radius:10px;background:linear-gradient(90deg,#0ea5a4,#06b6d4);color:#012;font-weight:700;text-decoration:none}
    .links a{display:block;color:var(--accent);text-decoration:none;margin-top:6px}
    footer{margin-top:36px;padding:18px 0;border-top:1px solid rgba(255,255,255,0.03);color:var(--muted);font-size:14px;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:8px}
    /* Gallery thumb */
    .thumb{width:100%;height:180px;border-radius:10px;overflow:hidden;background:linear-gradient(180deg, #041024, #02101a);display:flex;align-items:center;justify-content:center;color:var(--muted);font-size:13px}
    .thumb img{width:100%;height:100%;object-fit:cover;display:block}
    .resource-grid a{display:block;padding:14px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);text-decoration:none;color:inherit}
    .small{font-size:13px;color:var(--muted)}
    .center{display:flex;align-items:center;gap:10px}
    code{background:rgba(255,255,255,0.03);padding:2px 6px;border-radius:6px;font-family:ui-monospace, SFMono-Regular, Menlo, Monaco, 'Roboto Mono';font-size:13px}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">🌌</div>
        <div>
          <div style="font-weight:800">Espacio Exterior</div>
          <div class="small muted">Noticias, misiones y recursos oficiales</div>
        </div>
      </div>
      <nav>
        <a href="#misiones">Misiones</a>
        <a href="#galeria">Galería</a>
        <a href="#recursos">Recursos</a>
        <a href="#about">Acerca</a>
      </nav>
    </header>
    <!-- HERO -->
    <section class="hero">
      <div>
        <h1>Explora el Universo — recursos y misiones</h1>
        <p class="lead">Un punto de partida con enlaces oficiales y una galería de imágenes astronómicas. Ideal para aprender, presentar o compartir.</p>
        <div style="margin-top:18px" class="center">
          <a class="btn" href="#recursos">Ver recursos oficiales</a>
          <a class="btn" href="#galeria" style="background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--accent)">Abrir galería</a>
        </div>
        <div style="margin-top:22px" class="card small">
          <strong>Consejo:</strong> para usar imágenes reales guarda los archivos dentro de una carpeta `images/` en la misma carpeta que este `index.html`.
        </div>
      </div>
      <div class="card">
        <div style="font-weight:700">Imagen destacada</div>
        <div class="thumb" style="margin-top:12px">
          <!-- Si descargas imágenes, reemplaza el src por images/jwst.jpg -->
          <img src="https://www.nasa.gov/sites/default/files/thumbnails/image/webb_first_full_field.jpg" alt="JWST (imagen destacada) - NASA" onerror="this.style.display='none'">
          <div style="padding:14px;text-align:center;">
            <div class="muted">Si la imagen no carga, descarga desde los recursos oficiales (ver sección Recursos).</div>
          </div>
        </div>
      </div>
    </section>
    <!-- MISIONS -->
    <section id="misiones" style="margin-top:28px">
      <h2>Misiones destacadas</h2>
      <p class="muted">Breve guía de misiones históricas y actuales para empezar.</p>
      <div class="grid cols-3" style="margin-top:12px">
        <div class="card">
          <div style="font-weight:700">James Webb (JWST)</div>
          <div class="small muted" style="margin-top:8px">Telescopio espacial infrarrojo que observa galaxias distantes y formación estelar.</div>
          <div style="margin-top:10px"><a class="links" href="https://www.nasa.gov/mission_pages/webb/main/index.html" target="_blank" rel="noopener">Página NASA — JWST</a></div>
        </div>
        <div class="card">
          <div style="font-weight:700">Hubble Space Telescope</div>
          <div class="small muted" style="margin-top:8px">Décadas de imágenes icónicas del Universo visible.</div>
          <div style="margin-top:10px"><a class="links" href="https://www.nasa.gov/mission_pages/hubble/main/index.html" target="_blank" rel="noopener">Página NASA — Hubble</a></div>
        </div>
        <div class="card">
          <div style="font-weight:700">Mars Rovers (Curiosity / Perseverance)</div>
          <div class="small muted" style="margin-top:8px">Exploración y búsqueda de rastros de agua y vida pasada en Marte.</div>
          <div style="margin-top:10px"><a class="links" href="https://mars.nasa.gov" target="_blank" rel="noopener">Portal Mars (NASA)</a></div>
        </div>
      </div>
    </section>
    <!-- GALLERY -->
    <section id="galeria" style="margin-top:28px">
      <h2>Galería (sugerencias de imágenes)</h2>
      <p class="muted">Descarga imágenes oficiales desde los enlaces y reemplázalas en la carpeta `images/` si quieres usarlas localmente.</p>
      <div class="grid cols-3" style="margin-top:12px">
        <div class="card">
          <div style="font-weight:700">James Webb Telescope</div>
          <div class="thumb" style="margin-top:10px">
            <!-- placeholder: si pones images/jwst.jpg se mostrará -->
            <img src="images/jwst.jpg" alt="JWST (placeholder)" onerror="this.parentElement.innerHTML='<div class=\\'muted\\'>Reemplaza images/jwst.jpg con la imagen descargada desde NASA/ESA.</div>'">
          </div>
          <div class="small muted" style="margin-top:10px">Sugerido: descarga desde la biblioteca de imágenes de NASA/ESA.</div>
        </div>
        <div class="card">
          <div style="font-weight:700">Marte - Rover</div>
          <div class="thumb" style="margin-top:10px">
            <img src="images/mars_rover.jpg" alt="Rover Marte (placeholder)" onerror="this.parentElement.innerHTML='<div class=\\'muted\\'>Reemplaza images/mars_rover.jpg con la imagen descargada desde NASA.</div>'">
          </div>
          <div class="small muted" style="margin-top:10px">Perseverance / Curiosity — fotos oficiales disponibles públicamente.</div>
        </div>
        <div class="card">
          <div style="font-weight:700">Hubble — Nebulosas y galaxias</div>
          <div class="thumb" style="margin-top:10px">
            <img src="images/hubble.jpg" alt="Hubble (placeholder)" onerror="this.parentElement.innerHTML='<div class=\\'muted\\'>Reemplaza images/hubble.jpg con la imagen descargada desde Hubble site.</div>'">
          </div>
          <div class="small muted" style="margin-top:10px">Impresionantes composiciones a alta resolución.</div>
        </div>
      </div>
    </section>
    <!-- RESOURCES -->
    <section id="recursos" style="margin-top:28px">
      <h2>Recursos oficiales y enlaces recomendados</h2>
      <p class="muted">Enlaces directos a organismos y bibliotecas de imágenes oficiales (usa estos para descargar fotos y crédito):</p>
      <div class="grid cols-2" style="margin-top:12px">
        <div class="card resource-grid">
          <a href="https://www.nasa.gov" target="_blank" rel="noopener">NASA — Inicio</a>
          <a href="https://www.nasa.gov/multimedia/imagegallery/index.html" target="_blank" rel="noopener">NASA Image and Video Library</a>
          <a href="https://www.jpl.nasa.gov" target="_blank" rel="noopener">JPL (Jet Propulsion Laboratory)</a>
          <a href="https://mars.nasa.gov" target="_blank" rel="noopener">Portal Mars (misiones a Marte)</a>
        </div>
        <div class="card resource-grid">
          <a href="https://www.esa.int" target="_blank" rel="noopener">ESA — Agencia Espacial Europea</a>
          <a href="https://www.spacex.com" target="_blank" rel="noopener">SpaceX — Sitio oficial</a>
          <a href="https://www.isro.gov.in" target="_blank" rel="noopener">ISRO — Indian Space Research Organisation</a>
          <a href="https://en.wikipedia.org/wiki/Outer_space" target="_blank" rel="noopener">Wikipedia — Outer space (resumen)</a>
        </div>
      </div>
      <p class="small muted" style="margin-top:10px">Consejo: cuando uses una imagen de NASA/JPL/ESA para proyectos públicos, sigue la guía de atribución de la fuente que aparece en la misma página de la imagen.</p>
    </section>
    <!-- ABOUT -->
    <section id="about" style="margin-top:28px">
      <h2>Acerca de esta plantilla</h2>
      <p class="muted">Plantilla HTML estática creada como base — puedes personalizar textos, colores y añadir más secciones (blog, calendario de lanzamientos, etc.).</p>
      <div style="margin-top:12px" class="card small">
        <strong>Instrucciones rápidas para añadir imágenes locales</strong>
        <ol style="margin-top:8px">
          <li>Crear carpeta `images/` junto a este archivo `index.html`.</li>
          <li>Descargar imágenes (por ejemplo desde <a href="https://www.nasa.gov" target="_blank" rel="noopener">nasa.gov</a>) y guardarlas como `jwst.jpg`, `mars_rover.jpg`, `hubble.jpg`.</li>
          <li>Recarga la página; las miniaturas se mostrarán automáticamente si los nombres coinciden.</li>
        </ol>
      </div>
    </section>
    <footer>
      <div>© <span id="year"></span> Espacio Exterior — Recursos oficiales enlazados.</div>
      <div>Hecho por <strong>Jacquelin Moraima Garcilla Miranda</strong></div>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
