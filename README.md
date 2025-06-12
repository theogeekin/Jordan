<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Jordan Vault</title>
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: #111;
      color: #fff;
    }
    header {
      background: #000;
      padding: 20px;
      text-align: center;
    }
    nav a {
      color: red;
      margin: 0 15px;
      text-decoration: none;
    }
    .hero {
      padding: 60px;
      text-align: center;
      background: #222;
    }
    .shoe-grid {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
      padding: 40px;
    }
    .shoe-grid img {
      width: 200px;
      border-radius: 10px;
      transition: transform 0.3s;
    }
    .shoe-grid img:hover {
      transform: scale(1.05);
    }
    footer {
      text-align: center;
      padding: 20px;
      background: #000;
      color: #aaa;
    }
    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
      max-width: 400px;
      margin: 50px auto;
    }
    input, textarea, button {
      padding: 10px;
      font-size: 1em;
      border: none;
      border-radius: 5px;
    }
    button {
      background: red;
      color: white;
      cursor: pointer;
    }
    #intro {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: black;
      color: white;
      font-size: 2em;
      display: flex;
      align-items: center;
      justify-content: center;
      z-index: 9999;
    }
  </style>
</head>
<body>

  <!-- Intro Animation -->
  <div id="intro">
    🌍 Zooming to Virginia...
    <audio autoplay>
      <source src="intro-sound.mp3" type="audio/mp3">
      Your browser does not support the audio element.
    </audio>
  </div>

  <header>
    <h1>Jordan Vault</h1>
    <nav>
      <a href="#home">Home</a>
      <a href="#shop">Shop</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="home" class="hero">
    <h2>Legendary Air Jordans</h2>
    <p>Explore the iconic Air Jordan series 1–6.</p>
  </section>

  <section id="shop">
    <h3 style="text-align:center;">Shop Jordans</h3>
    <div class="shoe-grid">
      <img src="https://i.imgur.com/vNQX6VJ.jpg" alt="Jordan 1">
      <img src="https://i.imgur.com/XjOUHDh.jpg" alt="Jordan 2">
      <img src="https://i.imgur.com/E0xQp8P.jpg" alt="Jordan 3">
      <img src="https://i.imgur.com/sUeHe4B.jpg" alt="Jordan 4">
      <img src="https://i.imgur.com/pq2ezyY.jpg" alt="Jordan 5">
      <img src="https://i.imgur.com/2Dz4L4P.jpg" alt="Jordan 6">
    </div>
  </section>

  <section id="about">
    <h3 style="text-align:center;">About Jordan Vault</h3>
    <p style="max-width:600px;margin:auto;padding:20px;">
      Jordan Vault is a tribute to the legendary Air Jordan sneakers, showcasing the styles, stories, and culture behind Jordans 1 through 6. 
      Designed for sneakerheads who respect the classics and love the legacy.
    </p>
  </section>

  <section id="contact">
    <h3 style="text-align:center;">Contact Us</h3>
    <form>
      <input type="text" placeholder="Your Name" required/>
      <input type="email" placeholder="Email" required/>
      <textarea placeholder="Your message..." rows="5" required></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Jordan Vault. Not affiliated with Nike.</p>
  </footer>

  <script>
    window.onload = () => {
      setTimeout(() => {
        document.getElementById('intro').style.display = 'none';
      }, 4000); // 4-second intro
    };
  </script>

</body>
</html>