# WEBSITE-INDEX-HTML<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Fotofolio Pribadi</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      background: #f4f4f4;
      color: #333;
      line-height: 1.6;
      overflow-x: hidden;
    }

    header {
      background: #333;
      color: #fff;
      padding: 20px;
      text-align: center;
      animation: fadeInDown 1s ease-out;
    }

    header h1 {
      margin-bottom: 10px;
    }

    .profile-photo {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      border: 3px solid #fff;
      margin: 0 auto;
      display: block;
    }

    .about {
      padding: 20px;
      text-align: center;
      animation: fadeIn 1s ease-out;
    }

    .portfolio {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 15px;
      padding: 20px;
      animation: fadeInUp 1s ease-out;
    }

    .item {
      background: #fff;
      padding: 10px;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      transition: transform 0.3s, box-shadow 0.3s;
      cursor: pointer;
      opacity: 0;
      animation: itemFade 0.8s forwards;
    }

    .item:hover {
      transform: scale(1.05);
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
    }

    .item img {
      width: 100%;
      border-radius: 5px;
    }

    footer {
      text-align: center;
      padding: 20px;
      background: #333;
      color: #fff;
      animation: fadeIn 1s ease-out;
    }

    .btn-toggle {
      margin-top: 10px;
      padding: 8px 16px;
      background: #007bff;
      border: none;
      color: white;
      border-radius: 4px;
      cursor: pointer;
      transition: background 0.3s;
    }

    .btn-toggle:hover {
      background: #0056b3;
    }

    /* Animasi Keyframes */
    @keyframes fadeInDown {
      from {
        opacity: 0;
        transform: translateY(-30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(30px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }

    @keyframes itemFade {
      from {
        opacity: 0;
        transform: scale(0.95);
      }
      to {
        opacity: 1;
        transform: scale(1);
      }
    }

    /* Delay untuk animasi galeri */
    .item:nth-child(1) { animation-delay: 0.2s; }
    .item:nth-child(2) { animation-delay: 0.4s; }
    .item:nth-child(3) { animation-delay: 0.6s; }
    .item:nth-child(4) { animation-delay: 0.8s; }

  </style>
</head>
<body>

  <header>
    <img src="https://via.placeholder.com/120" alt="Foto Profil" class="profile-photo" />
    <h1>Nama Kamu</h1>
    <p>Fotografer | Desainer | Kreator Visual</p>
  </header>

  <section class="about">
    <h2>Tentang Saya</h2>
    <p>Halo! Saya adalah fotografer profesional yang suka menangkap momen istimewa melalui lensa kamera. Berikut adalah beberapa karya terbaik saya.</p>
    <button class="btn-toggle" onclick="togglePortfolio()">Tampilkan/Sembunyikan Karya</button>
  </section>

  <section class="portfolio" id="portfolio">
    <div class="item"><img src="https://via.placeholder.com/400x300?text=Karya+1" alt="Karya 1" /></div>
    <div class="item"><img src="https://via.placeholder.com/400x300?text=Karya+2" alt="Karya 2" /></div>
    <div class="item"><img src="https://via.placeholder.com/400x300?text=Karya+3" alt="Karya 3" /></div>
    <div class="item"><img src="https://via.placeholder.com/400x300?text=Karya+4" alt="Karya 4" /></div>
  </section>

  <footer>
    &copy; 2025 Nama Kamu. Semua Hak Dilindungi.
  </footer>

  <script>
    function togglePortfolio() {
      const portfolio = document.getElementById('portfolio');
      if (portfolio.style.display === 'none') {
        portfolio.style.display = 'grid';
      } else {
        portfolio.style.display = 'none';
      }
    }

    // Default tampil
    document.getElementById('portfolio').style.display = 'grid';
  </script>
</body>
</html>
