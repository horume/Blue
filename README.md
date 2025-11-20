# Blue
Quince años Azul
<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Zul - Quince Años</title>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
  <style>
    /* Reset básico */
    *{box-sizing:border-box;margin:0;padding:0}
    html,body{height:100%}
    body{
      font-family: "Inter", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      line-height:1.45;
      color:#222;
      background:#fff;
    }
    a{color:inherit;text-decoration:none}
    /* Layout */
    header{
      background:linear-gradient(180deg, rgba(255,255,255,0.6), rgba(255,255,255,0.3));
      backdrop-filter: blur(6px);
      position:sticky;top:0;z-index:40;
      border-bottom:1px solid rgba(0,0,0,0.05);
    }
    .container{max-width:1100px;margin:0 auto;padding:18px}
    .nav{
      display:flex;align-items:center;justify-content:space-between;gap:12px;
    }
    .brand{display:flex;align-items:center;gap:12px}
    .brand img{height:48px;width:auto;border-radius:8px}
    nav ul{display:flex;gap:16px;list-style:none;font-weight:600}
    /* Hero */
    .hero{
      display:grid;grid-template-columns:1fr;gap:24px;align-items:center;padding:48px 18px;
      background:linear-gradient(120deg,#f7f5ff 0%, #fff 60%);
    }
    .hero-inner{max-width:760px}
    .kicker{font-weight:600;color:#6b21a8;margin-bottom:8px}
    h1{font-family:"Playfair Display", serif;font-size:clamp(28px,4vw,42px);margin-bottom:12px}
    p.lead{color:#444;margin-bottom:18px}
    .cta{display:inline-block;padding:10px 18px;border-radius:10px;background:#6b21a8;color:white;font-weight:700}
    /* Grid de contenido */
    .grid{display:grid;grid-template-columns:repeat(2,1fr);gap:20px;padding:34px 18px}
    .card{background:#fff;border-radius:12px;box-shadow:0 6px 18px rgba(16,24,40,0.06);padding:18px}
    .media img{width:100%;height:auto;border-radius:8px}
    footer{padding:28px 18px;border-top:1px solid rgba(0,0,0,0.06);margin-top:24px}
    .center{text-align:center}
    /* responsive */
    @media (max-width:900px){
      .grid{grid-template-columns:1fr}
      nav ul{display:none}
    }
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">
        <!-- Reemplaza con el logo o imagen de tu Canva -->
        <img src="https://via.placeholder.com/120x60?text=Logo" alt="Logo">
        <div>
          <strong>Zul - Quince Años</strong><br>
          <small>Celebración · Invitación</small>
        </div>
      </div>
      <nav>
        <ul>
          <li><a href="#inicio">Inicio</a></li>
          <li><a href="#programa">Programa</a></li>
          <li><a href="#confirmar">Confirmar</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-inner">
        <div class="kicker">Invitación</div>
        <h1>Celebramos los XV años de Zul</h1>
        <p class="lead">Acompáñanos en una noche llena de alegría, música y recuerdos. Tu presencia nos honra.</p>
        <a class="cta" href="#confirmar">Confirmar asistencia</a>
      </div>
      <!-- Imagen hero: sustituye por tu exportación desde Canva -->
      <div style="padding:18px;">
        <img src="https://via.placeholder.com/720x480?text=Hero+Image" alt="Zul XV" style="width:100%;border-radius:12px;box-shadow:0 8px 30px rgba(0,0,0,0.08)">
      </div>
    </section>

    <section id="programa" class="container grid">
      <div class="card">
        <h3>Programa</h3>
        <p>Recepción — 18:00 hrs<br>Ceremonia — 19:00 hrs<br>Baile y cena — 20:00 hrs</p>
      </div>
      <div class="card">
        <h3>Ubicación</h3>
        <p>Salón Los Encinos<br>Dirección completa aquí</p>
      </div>

      <div class="card media">
        <img src="https://via.placeholder.com/600x360?text=Foto+1" alt="Foto evento">
      </div>
      <div class="card media">
        <img src="https://via.placeholder.com/600x360?text=Foto+2" alt="Foto evento">
      </div>
    </section>

    <section id="confirmar" class="container" style="padding:18px">
      <div class="card">
        <h3>Confirmar asistencia</h3>
        <p>Pulsa el botón para confirmar tu asistencia. Puedes añadir aquí un formulario o un enlace a RSVP.</p>

        <!-- Formulario simple (envío por correo via formsubmit o configurar Netlify) -->
        <form action="https://formsubmit.co/tu-correo@ejemplo.com" method="POST" style="display:grid;gap:12px;margin-top:12px">
          <input type="hidden" name="_next" value="https://tu-dominio.com/gracias.html">
          <input type="text" name="nombre" placeholder="Tu nombre" required style="padding:10px;border-radius:8px;border:1px solid #ddd">
          <select name="asistencia" required style="padding:10px;border-radius:8px;border:1px solid #ddd">
            <option value="">¿Asistirás?</option>
            <option value="si">Sí, asistiré</option>
            <option value="no">No podré asistir</option>
            <option value="talvez">Tal vez</option>
          </select>
          <button class="cta" type="submit" style="border:none;cursor:pointer">Confirmar asistencia</button>
        </form>

      </div>
    </section>

  </main>

  <footer class="center">
    <div class="container">
      <small>© 2025 Invitación · Todos los derechos reservados</small>
    </div>
  </footer>

</body>
</html>
