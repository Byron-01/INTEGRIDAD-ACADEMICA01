# INTEGRIDAD-ACADEMICA01
“Sitio web interactivo que promueve la integridad académica en estudiantes universitarios, con reflexiones personales, guía APA, buenas prácticas y recursos visuales para aprender y aplicar honestidad académica.”  
<html lang="es"><head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>SITE - Integridad Académica</title>
  <style>
    /* ---------- Reset & base ---------- */
    :root{
      --bg:#f7fafc; --card:#ffffff; --primary:#0f4c75; --accent:#00a8e8; --muted:#6b7280;
      --radius:12px; --max-width:1000px;
      font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    body{background:linear-gradient(180deg,var(--bg),#ffffff);margin:0;color:#102a43;}
    .container{max-width:var(--max-width);margin:32px auto;padding:20px}

    /* ---------- Header ---------- */
    header{display:flex;gap:16px;align-items:center;justify-content:space-between;margin-bottom:18px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:56px;height:56px;border-radius:10px;background:linear-gradient(135deg,var(--primary),var(--accent));display:flex;align-items:center;justify-content:center;color:white;font-weight:700}
    h1{font-size:20px;margin:0}
    p.lead{margin:0;color:var(--muted)}

    /* ---------- Tabs nav ---------- */
    nav{background:transparent;border-radius:10px;margin-bottom:18px}
    .tabs{display:flex;gap:8px;flex-wrap:wrap}
    .tab-btn{background:transparent;border:1px solid rgba(16,42,67,0.06);padding:10px 14px;border-radius:10px;cursor:pointer}
    .tab-btn.active{background:linear-gradient(90deg,var(--primary),var(--accent));color:white;border:none;box-shadow:0 6px 20px rgba(16,42,67,0.08)}

    /* ---------- Content cards ---------- */
    .card{background:var(--card);border-radius:var(--radius);padding:20px;box-shadow:0 6px 20px rgba(16,42,67,0.04);margin-bottom:16px}
    .grid{display:grid;grid-template-columns:1fr 380px;gap:18px}
    @media (max-width:900px){.grid{grid-template-columns:1fr}}

    .hero-img{height:180px;border-radius:10px;background:linear-gradient(90deg,rgba(0,168,232,0.12),rgba(15,76,117,0.08));display:flex;align-items:center;justify-content:center;color:var(--primary);font-weight:600}

    /* ---------- List & badges ---------- */
    ul.clean{padding-left:18px;margin:8px 0}
    .badge{display:inline-block;padding:6px 10px;border-radius:999px;font-size:13px;border:1px solid rgba(15,76,117,0.08);background:#fff}

    /* ---------- Gallery ---------- */
    .gallery{display:flex;flex-wrap:wrap;gap:10px}
    .photo{flex:1 1 110px;height:90px;border-radius:8px;background:#eef6fb;display:flex;align-items:center;justify-content:center;color:var(--muted);font-size:13px}

    /* ---------- CTA & footer ---------- */
    .cta{display:flex;gap:12px;align-items:center}
    .btn{background:var(--primary);color:white;padding:10px 14px;border-radius:10px;border:none;cursor:pointer}
    .btn.ghost{background:transparent;color:var(--primary);border:1px solid rgba(15,76,117,0.08)}

    footer{margin-top:24px;text-align:center;color:var(--muted);font-size:14px}

    /* ---------- Print friendly (cartulina) ---------- */
    @media print{
      body{background:white}
      nav, .btn, footer{display:none}
      .container{max-width:800px;margin:0;padding:0}
      .card{box-shadow:none;border-radius:0}
    }

  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">IA</div>
        <div>
          <h1>Sitio: Integridad Académica</h1>
          <p class="lead">Proyecto Site — Contenido original, guía APA y recursos visuales.</p>
        </div>
      </div>
      <div class="cta">
        <button class="btn" id="btn-download">Descargar HTML</button>
        <button class="btn ghost" id="btn-copy">Copiar contenido</button>
      </div>
    </header>

    <nav class="card">
      <div class="tabs" role="tablist" aria-label="Pestañas del sitio">
        <button class="tab-btn active" data-tab="inicio" aria-selected="true">Inicio</button>
        <button class="tab-btn" data-tab="experiencia" aria-selected="true">Mi experiencia</button>
        <button class="tab-btn" data-tab="buenas" aria-selected="true">Buenas prácticas</button>
        <button class="tab-btn" data-tab="apa" aria-selected="true">Mi guía APA</button>
        <button class="tab-btn" data-tab="referencias" aria-selected="true">Referencias</button>
      </div>
    </nav>

    <!-- ---------- Inicio ---------- -->
    <section id="inicio" class="card tabpanel" style="display: block;">
      <div class="grid">
        <div>
          <h2>¿Qué es la integridad académica?</h2>
          <p>La integridad académica es el compromiso con la honestidad, la responsabilidad y el respeto en todas las actividades académicas. Implica producir trabajo propio, citar fuentes correctamente y actuar con ética en evaluaciones y proyectos.</p>

          <h3>Frase lema</h3>
          <p class="badge">“La honestidad abre puertas, el plagio las cierra.”</p>

          <h3 style="margin-top:12px">Importancia</h3>
          <ul class="clean">
            <li>Protege el valor del título y del aprendizaje.</li>
            <li>Fomenta la confianza entre estudiantes y docentes.</li>
            <li>Prepara profesionales responsables y éticos.</li>
          </ul>
        </div>

        <aside>
          <div class="hero-img">Aquí va una infografía (reemplaza por imagen)</div>
          <p style="margin-top:10px;color:var(--muted);font-size:14px">Consejo: crea una infografía en Canva (tamaño: 800×450) con íconos de libro, candado y estudiantes.</p>
        </aside>
      </div>
    </section>

    <!-- ---------- Mi experiencia personal ---------- -->
    <section id="experiencia" class="card tabpanel" style="display: none;">
      <h2>Mi experiencia personal</h2>
      <div class="grid">
        <div>
          <h3>Relato</h3>
          <p>Durante un examen, un compañero me ofreció sus respuestas. Me sentí tentado, pero decidí resolverlo con lo que había estudiado. Aunque la nota no fue perfecta, la tranquilidad y el aprendizaje propio valieron la pena.</p>

          <h3>Reflexión</h3>
          <p>Esta experiencia me recordó que la integridad académica fortalece mi identidad como estudiante y profesional. Mantener principios éticos me ayuda a construir confianza y credibilidad.</p>

          <h3>Video personal (2 min)</h3>
          <p>Inserta aquí un video corto con tu reflexión. Si lo subes a YouTube, pega el enlace en el iframe siguiente (o sustituye por tu archivo en el hosting elegido).</p>

          <!-- Placeholder YouTube iframe - reemplaza src con tu video -->
          <div style="margin-top:8px">
            <iframe width="100%" height="220" src="https://www.youtube.com/embed/VIDEO_ID" title="Video personal" frameborder="0" allowfullscreen="" style="border-radius:8px"></iframe>
          </div>

        </div>

        <aside>
          <div class="card">
            <h4>Guía rápida</h4>
            <ol>
              <li>Escribe el guion de menos de 2 minutos.</li>
              <li>Graba con luz natural y voz clara.</li>
              <li>Sube a YouTube en modo oculto o privado y pega el enlace.</li>
            </ol>
          </div>

          <div style="height:12px"></div>

          <div class="card">
            <h4>Pregunta para reflexión</h4>
            <p class="muted">¿Cómo afecta esta decisión a tu confianza académica a futuro?</p>
          </div>
        </aside>
      </div>
    </section>

    <!-- ---------- Buenas prácticas ---------- -->
    <section id="buenas" class="card tabpanel" style="display: none;">
      <h2>Buenas prácticas de integridad académica</h2>
      <div class="grid">
        <div>
          <h3>Lista de buenas prácticas</h3>
          <ul class="clean">
            <li>Citar siempre las fuentes y usar comillas cuando corresponda.</li>
            <li>Planificar el estudio para evitar el trabajo de última hora.</li>
            <li>Evitar compartir respuestas en evaluaciones.</li>
            <li>Usar gestores bibliográficos (Zotero, Mendeley) para organizar referencias.</li>
            <li>Revisar las normas de la universidad sobre integridad y sanciones.</li>
          </ul>

          <h3>Acciones pequeñas que marcan la diferencia</h3>
          <ul class="clean">
            <li>Guardar tus borradores y fechas de entrega.</li>
            <li>Pedir una aclaración al docente cuando algo no está claro.</li>
            <li>Trabajar en equipo con roles y evidencias claras.</li>
          </ul>

          <h3>Eslogan visual</h3>
          <p class="badge" style="margin-top:8px">Sé original, sé íntegro, sé tú.</p>
        </div>

        <aside>
          <h4>Galería</h4>
          <div class="gallery">
            <div class="photo">Icono: citar</div>
            <div class="photo">Icono: estudiar</div>
            <div class="photo">Icono: equipo</div>
            <div class="photo">Icono: confianza</div>
          </div>

          <div style="height:12px"></div>

          <div class="card">
            <h4>Hoja de actividades</h4>
            <p>Incluye ejercicios: identificar plagio, reescribir parafraseo, practicar citas APA.</p>
          </div>
        </aside>
      </div>
    </section>

    <!-- ---------- Guía APA y confiabilidad ---------- -->
    <section id="apa" class="card tabpanel" style="display: none;">
      <h2>Mi guía APA y confiabilidad académica</h2>

      <h3>¿Qué es una fuente confiable?</h3>
      <p>Son fuentes de instituciones académicas, artículos revisados por pares, libros de editoriales reconocidas y sitios oficiales. Criterios: autor conocido, fecha, editorial o revista, revisión por pares y transparencia metodológica.</p>

      <h3>Tipos de fuentes</h3>
      <ul class="clean">
        <li><strong>Primarias:</strong> estudios originales, tesis, datos brutos.</li>
        <li><strong>Secundarias:</strong> revisiones, análisis, libros de texto.</li>
        <li><strong>Terciarias:</strong> enciclopedias, resúmenes.</li>
      </ul>

      <h3>Ejemplos de citas en APA 7ª</h3>
      <div style="background:#fbfdff;padding:12px;border-radius:8px;margin-bottom:12px">
        <p><strong>Libro:</strong><br>
        Ausubel, D. (2002). <em>Psicología educativa: Un punto de vista cognoscitivo</em>. Trillas.</p>

        <p><strong>Artículo web:</strong><br>
        UNESCO. (2023). <em>La integridad académica como valor</em>. https://www.unesco.org/</p>

        <p><strong>Artículo científico:</strong><br>
        Smith, J. (2021). Academic honesty in higher education. <em>Journal of Education, 15</em>(3), 45–60.</p>
      </div>

      <h3>Cómo hacer una lista de referencias</h3>
      <p>Ordena alfabéticamente por apellido del autor; usa sangría francesa (hanging indent) y asegúrate de incluir DOI cuando exista.</p>

      <h3>Generadores de citas y recursos</h3>
      <ul class="clean">
        <li>Zotero — gestor bibliográfico.</li>
        <li>Mendeley — gestor y red académica.</li>
        <li>Citation Machine / CiteThisForMe — generadores rápidos.</li>
      </ul>

      <h3>Video tutorial</h3>
      <p>Puedes crear un pequeño screencast (2–3 min) mostrando cómo copiar una referencia y formatearla en APA 7ª.</p>
    </section>

    <!-- ---------- Referencias (APA) ---------- -->
    <section id="referencias" class="card tabpanel" style="display: none;">
      <h2>Referencias</h2>
      <ol>
        <li>Ausubel, D. (2002). <em>Psicología educativa: Un punto de vista cognoscitivo</em>. Trillas.</li>
        <li>UNESCO. (2023). <em>La integridad académica como valor</em>. https://www.unesco.org/</li>
        <li>Vygotsky, L. S. (1979). <em>El desarrollo de los procesos psicológicos superiores</em>. Crítica.</li>
      </ol>

      <p style="margin-top:12px;color:var(--muted)">Nota: reemplaza las referencias por las fuentes exactas que consultes y añade DOI cuando corresponda.</p>
    </section>

    <footer>
      Creado por: [Tu nombre] • Proyecto SITE • Edita el contenido antes de publicar
    </footer>
  </div>

  <script>
    // ---------- Tab navigation ----------
    const tabs = document.querySelectorAll('.tab-btn');
    const panels = document.querySelectorAll('.tabpanel');
    tabs.forEach(btn=>btn.addEventListener('click',()=>{
      tabs.forEach(b=>b.classList.remove('active'));
      btn.classList.add('active');
      const tab = btn.dataset.tab;
      panels.forEach(p=>p.style.display = p.id === tab ? 'block' : 'none');
      // for accessibility
      btn.setAttribute('aria-selected','true');
    }));

    // ---------- Download HTML ----------
    document.getElementById('btn-download').addEventListener('click',()=>{
      const content = '<!doctype html>\n' + document.documentElement.outerHTML;
      const blob = new Blob([content],{type:'text/html'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a'); a.href = url; a.download = 'SITE_Integridad_Academica.html'; document.body.appendChild(a); a.click(); a.remove(); URL.revokeObjectURL(url);
    });

    // ---------- Copy content ----------
    document.getElementById('btn-copy').addEventListener('click',async ()=>{
      try{
        await navigator.clipboard.writeText(document.documentElement.outerHTML);
        alert('HTML copiado al portapapeles. Pégalo en tu editor o en Canva (si usas la opción de subir código).');
      }catch(e){
        alert('No se pudo copiar automáticamente. Usa Descargar HTML.');
      }
    });
  </script>

  <!--
    INSTRUCCIONES para Canva / subir a un host
    - Si vas a usar Canva Websites: crea una página en blanco y copia el texto/imagenes manualmente.
    - Para mantener el diseño tal cual: descarga este archivo HTML y súbelo a un hosting (GitHub Pages, Netlify) o abre localmente.
    - Para exportar a cartulina: usa la vista de impresión (Ctrl+P) y selecciona "Guardar como PDF" con tamaño A3 o similar.
    - Reemplaza los placeholders (infografía, VIDEO_ID, fotos) por tus recursos reales.
  -->


</body></html>
