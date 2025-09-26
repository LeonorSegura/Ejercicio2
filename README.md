<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Conoce-T Centro Psicológico y Psicoanalítico</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-image: url('https://github.com/Per-Arredondo/Clinica_medica/blob/main/Fondo%20JPG.jpeg?raw=true');
      background-size: cover;
      background-attachment: fixed;
      color: #333;
    }
    header {
      background: rgba(255, 255, 255, 0.9);
      text-align: center;
      padding: 1rem;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    }
    header img {
      max-height: 100px;
    }
    .banner {
      width: 100%;
      height: auto;
      display: block;
    }
    section {
      background: rgba(255, 255, 255, 0.95);
      margin: 2rem;
      padding: 1.5rem;
      border-radius: 20px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    }
    h2 {
      color: #6a1b9a;
    }
    .accordion {
      cursor: pointer;
      padding: 1rem;
      background: #e3f2fd;
      border-radius: 15px;
      margin-top: 10px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    .panel {
      display: none;
      padding: 0.5rem 1rem;
      background: #f8f9fa;
      border-radius: 10px;
      margin-top: 5px;
    }
    form {
      display: grid;
      gap: 1rem;
    }
    input, select, textarea, button {
      padding: 0.75rem;
      border-radius: 10px;
      border: 1px solid #ccc;
      font-size: 1rem;
    }
    button {
      background: #6a1b9a;
      color: white;
      border: none;
      cursor: pointer;
    }
    .success-message {
      color: green;
      font-weight: bold;
      margin-top: 1rem;
      display: none;
    }
    .social-links a {
      margin: 0 10px;
      text-decoration: none;
      color: #6a1b9a;
      font-weight: bold;
    }
    @media(max-width: 768px){
      section {
        margin: 1rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <img src="C:\\Users\\leo_s\\Downloads\\Logo Conocet.png" alt="Logo Conoce-T" />
  </header>
  <img class="banner" src="C:\\Users\\leo_s\\Downloads\\BannerConocet.png" alt="Banner Conoce-T" />

  <section>
    <h2>¿Quiénes somos?</h2>
    <p>Somos un espacio dedicado a la Supervisión y crecimiento de terapeutas, así como el acompañamiento de quienes buscan conocerse y sanar a través del psicoanálisis...</p>
  </section>

  <section>
    <h2>Misión</h2>
    <p>Refinar la manera en que los terapeutas comprenden a sus pacientes...</p>
  </section>

  <section>
    <h2>Visión</h2>
    <p>Ser una clínica referente por excelencia, trato humano y compromiso con la salud mental.</p>
  </section>

  <section>
    <h2>Valores</h2>
    <p><strong>Compromiso con la salud mental:</strong> Creemos en la Psicoterapia-Psicoanálisis como un proceso de transformación genuina...</p>
  </section>

  <section>
    <h2>Terapia Psicoanalítica</h2>
    <div class="accordion">Psicoterapia para Parejas</div>
    <div class="panel">Atención enfocada en dinámicas relacionales y comunicación efectiva.</div>

    <div class="accordion">Psicoterapia para Niños</div>
    <div class="panel">Espacio terapéutico especializado en el desarrollo emocional infantil.</div>

    <div class="accordion">Psicoterapia para Adolescentes</div>
    <div class="panel">Intervenciones centradas en identidad, autoestima y vínculos.</div>

    <div class="accordion">Psicoterapia Individual</div>
    <div class="panel">Proceso de autoconocimiento profundo y elaboración emocional.</div>

    <div class="accordion">Supervisión de Casos Clínicos</div>
    <div class="panel">Espacio de aprendizaje, reflexión clínica y crecimiento profesional.</div>
  </section>

  <section>
    <h2>Agendar Cita</h2>
    <form id="citaForm">
      <input type="text" name="nombre" placeholder="Nombre completo" required />
      <input type="tel" name="telefono" placeholder="Teléfono" required />
      <input type="email" name="correo" placeholder="Correo electrónico" required />
      <select name="sexo" required>
        <option value="">Sexo</option>
        <option value="Femenino">Femenino</option>
        <option value="Masculino">Masculino</option>
        <option value="Otro">Otro</option>
      </select>
      <select name="tipo_terapia" required>
        <option value="">Tipo de Terapia</option>
        <option>Psicoterapia para Parejas</option>
        <option>Psicoterapia para Niños</option>
        <option>Psicoterapia para Adolescentes</option>
        <option>Psicoterapia Individual</option>
        <option>Supervisión de Casos Clínicos</option>
      </select>
      <input type="date" name="fecha" required />
      <input type="time" name="hora" required />
      <textarea name="comentarios" placeholder="Comentarios adicionales"></textarea>
      <button type="submit">Agendar</button>
      <div class="success-message" id="mensajeExito"></div>
    </form>
  </section>

  <section class="social-links">
    <h2>Síguenos en nuestras redes sociales</h2>
    <a href="https://instagram.com/conocet.psi?igsh=MWhnMXhkcHI1aGU0Yg" target="_blank">Instagram</a>
    <a href="https://facebook.com/profile.php?id=100041276426768&mibextid=ZbWKwL" target="_blank">Facebook</a>
    <a href="https://youtube.com/@danarova1?si=iAvCTihSSI7VcsCq" target="_blank">YouTube</a>
    <a href="https://tiktok.com/@centroconocet?_t=8nOLvJV1PYT&_r=1" target="_blank">TikTok</a>
  </section>

  <script>
    // Acordeón terapias
    document.querySelectorAll('.accordion').forEach(acc => {
      acc.addEventListener('click', () => {
        const panel = acc.nextElementSibling;
        panel.style.display = panel.style.display === 'block' ? 'none' : 'block';
      });
    });

    // Envío del formulario
    document.getElementById('citaForm').addEventListener('submit', function(e) {
      e.preventDefault();
      const form = e.target;
      const data = new FormData(form);

      fetch('https://script.google.com/macros/s/AKfycbwqkIOnrvtAlrmEtrGKkGku2HvRWF5fkBIkEIxtMuOcVLEMJiTs28IfXWPCAhge6m1Kow/exec', {
        method: 'POST',
        body: data
      })
      .then(res => res.ok ? res : Promise.reject())
      .then(() => {
        const msg = document.getElementById('mensajeExito');
        msg.innerHTML = '✅ Gracias, tu cita ha sido agendada.<br>⏳ Redirigiendo al inicio...<br>🎉 Te contactaremos pronto.';
        msg.style.display = 'block';
        form.reset();
        window.scrollTo({ top: 0, behavior: 'smooth' });
        setTimeout(() => {
          msg.style.display = 'none';
        }, 5000);
      })
      .catch(() => alert('Error al enviar. Intente más tarde.'));
    });
  </script>
</body>
</html>
