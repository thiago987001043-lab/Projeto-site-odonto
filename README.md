```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <title>Clínica Odontológica Maria Clara | Dentista Especializada</title>
  <meta name="description" content="Clínica odontológica da Dra. Maria Clara. Agende consultas online, tratamentos estéticos, ortodontia, limpeza dental e atendimento humanizado." />
  <meta name="keywords" content="dentista, clínica odontológica, Maria Clara, clareamento dental, ortodontia, implante dentário" />
  <meta name="author" content="Maria Clara" />

  <!-- SEO -->
  <meta property="og:title" content="Clínica Maria Clara" />
  <meta property="og:description" content="Atendimento odontológico premium com tecnologia moderna." />
  <meta property="og:type" content="website" />

  <!-- Analytics -->
  <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
  <script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'G-XXXXXXXXXX');
  </script>

  <!-- Icons -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont@latest/tabler-icons.min.css">

  <!-- Font -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    :root {
      --bg: #f8fafc;
      --surface: #ffffff;
      --primary: #2563eb;
      --primary-light: #60a5fa;
      --secondary: #0f172a;
      --text: #1e293b;
      --muted: #64748b;
      --border: #e2e8f0;
      --success: #22c55e;
      --shadow: 0 10px 30px rgba(0,0,0,.08);
      --radius: 18px;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: var(--bg);
      color: var(--text);
      overflow-x: hidden;
    }

    header {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 999;
      backdrop-filter: blur(14px);
      background: rgba(255,255,255,.85);
      border-bottom: 1px solid var(--border);
    }

    .navbar {
      max-width: 1200px;
      margin: auto;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 18px 20px;
    }

    .logo {
      font-size: 1.4rem;
      font-weight: 800;
      color: var(--secondary);
    }

    .logo span {
      color: var(--primary);
    }

    .nav-links {
      display: flex;
      gap: 24px;
      list-style: none;
    }

    .nav-links a {
      text-decoration: none;
      color: var(--text);
      font-weight: 500;
      transition: .3s;
    }

    .nav-links a:hover {
      color: var(--primary);
    }

    .btn {
      background: var(--primary);
      color: white;
      border: none;
      padding: 14px 24px;
      border-radius: 12px;
      font-weight: 600;
      cursor: pointer;
      transition: .3s;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }

    .btn:hover {
      transform: translateY(-2px);
      background: #1d4ed8;
    }

    .hero {
      min-height: 100vh;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      align-items: center;
      gap: 50px;
      max-width: 1200px;
      margin: auto;
      padding: 140px 20px 80px;
    }

    .hero-text h1 {
      font-size: 4rem;
      line-height: 1.1;
      margin-bottom: 20px;
      color: var(--secondary);
    }

    .hero-text p {
      font-size: 1.1rem;
      color: var(--muted);
      line-height: 1.7;
      margin-bottom: 32px;
    }

    .hero-image {
      position: relative;
    }

    .hero-image img {
      width: 100%;
      border-radius: 30px;
      box-shadow: var(--shadow);
    }

    .stats {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
      max-width: 1200px;
      margin: auto;
      padding: 40px 20px;
    }

    .stat-card {
      background: var(--surface);
      border-radius: var(--radius);
      padding: 28px;
      box-shadow: var(--shadow);
      border: 1px solid var(--border);
    }

    .stat-card h3 {
      font-size: 2rem;
      color: var(--primary);
      margin-bottom: 8px;
    }

    .section {
      max-width: 1200px;
      margin: auto;
      padding: 100px 20px;
    }

    .section-title {
      text-align: center;
      margin-bottom: 60px;
    }

    .section-title h2 {
      font-size: 2.8rem;
      margin-bottom: 12px;
      color: var(--secondary);
    }

    .section-title p {
      color: var(--muted);
      max-width: 700px;
      margin: auto;
      line-height: 1.7;
    }

    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 24px;
    }

    .service-card {
      background: white;
      border-radius: var(--radius);
      padding: 32px;
      border: 1px solid var(--border);
      transition: .3s;
      box-shadow: var(--shadow);
    }

    .service-card:hover {
      transform: translateY(-8px);
    }

    .service-card i {
      font-size: 2.5rem;
      color: var(--primary);
      margin-bottom: 18px;
    }

    .service-card h3 {
      margin-bottom: 14px;
    }

    .dashboard {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .dashboard-card {
      background: white;
      border-radius: var(--radius);
      padding: 28px;
      box-shadow: var(--shadow);
      border: 1px solid var(--border);
    }

    .dashboard-card h4 {
      color: var(--muted);
      margin-bottom: 12px;
      font-size: .95rem;
    }

    .dashboard-card h2 {
      font-size: 2.2rem;
      color: var(--secondary);
    }

    .appointment {
      background: linear-gradient(135deg, #2563eb, #1e3a8a);
      border-radius: 30px;
      padding: 60px;
      color: white;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 40px;
      align-items: center;
    }

    .appointment-form {
      display: flex;
      flex-direction: column;
      gap: 16px;
    }

    .appointment-form input,
    .appointment-form select,
    .appointment-form textarea {
      padding: 16px;
      border-radius: 12px;
      border: none;
      outline: none;
      font-family: inherit;
    }

    .appointment-form button {
      background: white;
      color: var(--primary);
      border: none;
      padding: 16px;
      border-radius: 12px;
      font-weight: 700;
      cursor: pointer;
      transition: .3s;
    }

    .appointment-form button:hover {
      transform: scale(1.02);
    }

    footer {
      background: var(--secondary);
      color: white;
      padding: 70px 20px;
      margin-top: 80px;
    }

    .footer-content {
      max-width: 1200px;
      margin: auto;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }

    .footer-content h3 {
      margin-bottom: 20px;
    }

    .footer-content p,
    .footer-content a {
      color: #cbd5e1;
      text-decoration: none;
      line-height: 1.8;
    }

    .floating-whatsapp {
      position: fixed;
      right: 24px;
      bottom: 24px;
      width: 65px;
      height: 65px;
      border-radius: 50%;
      background: #25d366;
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2rem;
      text-decoration: none;
      box-shadow: var(--shadow);
      z-index: 999;
    }

    @media(max-width: 768px){
      .hero-text h1 {
        font-size: 2.8rem;
      }

      .nav-links {
        display: none;
      }

      .appointment {
        padding: 30px;
      }
    }
  </style>
</head>
<body>

<header>
  <nav class="navbar">
    <div class="logo">Maria <span>Clara</span></div>

    <ul class="nav-links">
      <li><a href="#inicio">Início</a></li>
      <li><a href="#servicos">Serviços</a></li>
      <li><a href="#dashboard">Dashboard</a></li>
      <li><a href="#agendamento">Agendamento</a></li>
      <li><a href="#contato">Contato</a></li>
    </ul>

    <a href="#agendamento" class="btn">
      <i class="ti ti-calendar"></i>
      Agendar
    </a>
  </nav>
</header>

<section class="hero" id="inicio">
  <div class="hero-text">
    <h1>Sorrisos saudáveis começam aqui.</h1>

    <p>
      Atendimento odontológico moderno, humanizado e tecnológico.
      A Dra. Maria Clara oferece tratamentos premium para transformar sua saúde bucal e autoestima.
    </p>

    <a href="#agendamento" class="btn">
      <i class="ti ti-stethoscope"></i>
      Agendar Consulta
    </a>
  </div>

  <div class="hero-image">
    <img src="https://images.unsplash.com/photo-1629909613654-28e377c37b09?q=80&w=1200&auto=format&fit=crop" alt="Dentista Maria Clara">
  </div>
</section>

<section class="stats">
  <div class="stat-card">
    <h3>+5 Mil</h3>
    <p>Pacientes atendidos</p>
  </div>

  <div class="stat-card">
    <h3>98%</h3>
    <p>Satisfação dos clientes</p>
  </div>

  <div class="stat-card">
    <h3>12 Anos</h3>
    <p>De experiência clínica</p>
  </div>

  <div class="stat-card">
    <h3>24/7</h3>
    <p>Suporte online</p>
  </div>
</section>

<section class="section" id="servicos">
  <div class="section-title">
    <h2>Nossos Serviços</h2>
    <p>
      Tratamentos completos para cuidar do seu sorriso com excelência.
    </p>
  </div>

  <div class="services">
    <div class="service-card">
      <i class="ti ti-brush"></i>
      <h3>Limpeza Dental</h3>
      <p>Prevenção e higienização completa para sua saúde bucal.</p>
    </div>

    <div class="service-card">
      <i class="ti ti-star"></i>
      <h3>Clareamento</h3>
      <p>Procedimentos estéticos modernos e seguros.</p>
    </div>

    <div class="service-card">
      <i class="ti ti-heart"></i>
      <h3>Implantes</h3>
      <p>Recupere seu sorriso com implantes de alta qualidade.</p>
    </div>

    <div class="service-card">
      <i class="ti ti-align-box-left-middle"></i>
      <h3>Ortodontia</h3>
      <p>Aparelhos e alinhadores modernos para todas as idades.</p>
    </div>
  </div>
</section>

<section class="section" id="dashboard">
  <div class="section-title">
    <h2>Dashboard Inteligente</h2>
    <p>
      Indicadores de desempenho e gestão clínica em tempo real.
    </p>
  </div>

  <div class="dashboard">
    <div class="dashboard-card">
      <h4>Consultas Hoje</h4>
      <h2 id="appointments">24</h2>
    </div>

    <div class="dashboard-card">
      <h4>Novos Pacientes</h4>
      <h2 id="patients">12</h2>
    </div>

    <div class="dashboard-card">
      <h4>Avaliação Média</h4>
      <h2>4.9★</h2>
    </div>

    <div class="dashboard-card">
      <h4>Taxa de Retorno</h4>
      <h2>87%</h2>
    </div>
  </div>
</section>

<section class="section" id="agendamento">
  <div class="appointment">
    <div>
      <h2 style="font-size:3rem;margin-bottom:20px">
        Agende sua consulta.
      </h2>

      <p style="line-height:1.8;font-size:1.05rem">
        Atendimento personalizado com tecnologia avançada e conforto premium.
      </p>
    </div>

    <form class="appointment-form" id="appointmentForm">
      <input type="text" placeholder="Nome completo" required>
      <input type="email" placeholder="E-mail" required>
      <input type="tel" placeholder="Telefone" required>

      <select required>
        <option value="">Escolha um serviço</option>
        <option>Clareamento</option>
        <option>Ortodontia</option>
        <option>Implante</option>
        <option>Limpeza</option>
      </select>

      <textarea rows="5" placeholder="Observações"></textarea>

      <button type="submit">
        Confirmar Agendamento
      </button>
    </form>
  </div>
</section>

<footer id="contato">
  <div class="footer-content">
    <div>
      <h3>Maria Clara</h3>
      <p>
        Clínica odontológica premium focada em saúde, estética e tecnologia.
      </p>
    </div>

    <div>
      <h3>Contato</h3>
      <p>📍 Campina Grande - PB</p>
      <p>📞 (83) 99999-9999</p>
      <p>✉️ contato@mariaclara.com</p>
    </div>

    <div>
      <h3>Horários</h3>
      <p>Seg - Sex: 08h às 18h</p>
      <p>Sábado: 08h às 13h</p>
    </div>
  </div>
</footer>

<a class="floating-whatsapp" href="https://wa.me/5583999999999" target="_blank">
  <i class="ti ti-brand-whatsapp"></i>
</a>

<script>
  // Dashboard animation
  const animateValue = (id, start, end, duration) => {
    let current = start;
    const range = end - start;
    const increment = end > start ? 1 : -1;
    const stepTime = Math.abs(Math.floor(duration / range));

    const obj = document.getElementById(id);

    const timer = setInterval(() => {
      current += increment;
      obj.textContent = current;

      if (current === end) {
        clearInterval(timer);
      }
    }, stepTime);
  }

  window.addEventListener('load', () => {
    animateValue('appointments', 0, 24, 1200);
    animateValue('patients', 0, 12, 1400);
  });

  // Appointment form
  document.getElementById('appointmentForm').addEventListener('submit', function(e){
    e.preventDefault();

    alert('Consulta agendada com sucesso! Entraremos em contato em breve.');

    this.reset();
  });

  // Scroll effect navbar
  window.addEventListener('scroll', () => {
    const header = document.querySelector('header');

    if(window.scrollY > 40){
      header.style.boxShadow = '0 10px 30px rgba(0,0,0,.08)';
    } else {
      header.style.boxShadow = 'none';
    }
  });
</script>

</body>
</html>
