<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Portofolio Saya</title>
  <style>
    html {
      scroll-behavior: smooth;
    }
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(to right, #00c6ff, #0072ff);
      color: white;
    }
    header {
      padding: 20px;
      text-align: center;
      background-color: rgba(0, 0, 0, 0.2);
      animation: slideDown 1s ease-out;
    }
    nav {
      margin-top: 10px;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }
    nav a:hover {
      text-decoration: underline;
      color: #ffd700;
    }
    section {
      padding: 80px 20px;
      text-align: center;
    }
    .hero {
      animation: scaleFade 1.2s ease-out;
      padding-top: 100px;
    }
    #tentang {
      animation: slideLeft 1.2s ease-out;
    }
    #proyek {
      animation: slideRight 1.2s ease-out;
    }
    #kontak {
      animation: fadeIn 1.2s ease-out;
    }
    footer {
      text-align: center;
      padding: 20px;
      background-color: rgba(0, 0, 0, 0.2);
      position: fixed;
      bottom: 0;
      width: 100%;
      animation: fadeIn 2s ease-in-out;
    }

    /* Form styling */
    input, textarea {
      padding: 10px;
      width: 80%;
      max-width: 400px;
      margin-bottom: 10px;
      border: none;
      border-radius: 5px;
    }
    button {
      padding: 10px 20px;
      background-color: #ffd700;
      border: none;
      border-radius: 5px;
      cursor: not-allowed;
      opacity: 0.6;
    }

    .social a {
      color: white;
      margin: 0 10px;
      font-weight: bold;
      display: inline-block;
      transition: transform 0.3s, color 0.3s;
    }
    .social a:hover {
      color: #ffd700;
      transform: translateY(-3px);
    }

    /* Animations */
    @keyframes slideDown {
      0% { transform: translateY(-50px); opacity: 0; }
      100% { transform: translateY(0); opacity: 1; }
    }
    @keyframes slideLeft {
      0% { transform: translateX(-100px); opacity: 0; }
      100% { transform: translateX(0); opacity: 1; }
    }
    @keyframes slideRight {
      0% { transform: translateX(100px); opacity: 0; }
      100% { transform: translateX(0); opacity: 1; }
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    @keyframes scaleFade {
      0% { transform: scale(0.8); opacity: 0; }
      100% { transform: scale(1); opacity: 1; }
    }
  </style>
</head>
<body>

  <header>
    <h1>Selamat Datang di Portofolio Saya</h1>
    <nav>
      <a href="#beranda">Beranda</a>
      <a href="#tentang">Tentang Saya</a>
      <a href="#proyek">Proyek</a>
      <a href="#kontak">Kontak</a>
    </nav>
  </header>

  <section id="beranda" class="hero">
   <img src="poto.jpg" alt="profile-irfan" style="width: 200px; height: 200px; border-radius: 100%; object-fit: cover;">
    <h1>Halo, saya Irfan dwi A.!</h1>
    <p>Saya adalah web developer yang fokus pada front-end development dan desain UI/UX.</p>
  </section>

  <section id="tentang">
    <h2>Tentang Saya</h2>
    <p>Saya adalah seorang pengembang web dengan minat dalam membuat tampilan antarmuka yang menarik dan responsif. Saya memiliki pengalaman dalam HTML, CSS, JavaScript, dan beberapa framework seperti React.</p>
  </section>

  <section id="proyek">
    <h2>Proyek</h2>
    <p>Berikut beberapa proyek yang pernah saya kerjakan:</p>
    <ul style="list-style: none; padding: 0;">
      <li>- Website Portfolio Pribadi</li>
      <li>- Aplikasi To-Do List dengan React</li>
      <li>- Desain UI untuk aplikasi e-commerce</li>
    </ul>
  </section>

  <section id="kontak">
    <h2>Kontak</h2>
    <p>Anda dapat menghubungi saya melalui WhatsApp di <a href="https://wa.me/62882005509840" style="color: #ffd700;">+62 882-0055-09840</a></p>

    <form onsubmit="alert('Terima kasih! Pesan Anda telah dikirim. (simulasi)'); return false;">
  <input type="text" name="name" placeholder="Nama Anda" required><br>
  <input type="text" name="phone" placeholder="Nomor HP Anda" required><br>
  <textarea name="message" placeholder="Pesan Anda" required></textarea><br>
  <button type="submit">Kirim</button>
</form>

<div class="social" style="margin-top: 20px;">
      <a href="https://github.com/ipan-2009" target="_blank">github</a>
      <a href="https://www.instagram.com/panpanzzz2" target="_blank">instragram</a>
      <a href="https://tiktok.com/@iponzzzyy" target="_blank">tiktok</a>
    </div>
  </section>

  <footer>
    &copy; 2025 irfan. Semua hak dilindungi.
  </footer>

</body>
</html>
