** COMPANY **: CODTECH IT SOLUTIONS

** NAME **: Ashija Kotian

** INTERN ID **: CT04DY1059

** DOMAIN **: UI/UX DESIGN

** DURATION **: 4 WEEKS

** MENTOR **: NEELA SANTOSH

CODE:
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Restaurant Landing Page</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
    }
    /* Navbar */
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      background: #8B0000;
      color: #fff;
    }
    nav ul {
      display: flex;
      list-style: none;
    }
    nav ul li {
      margin: 0 15px;
    }
    nav ul li a {
      color: #fff;
      text-decoration: none;
    }
    .menu-toggle {
      display: none;
      font-size: 24px;
      cursor: pointer;
    }

    /* Hero */
    .hero {
      background: url('https://images.unsplash.com/photo-1600891964092-4316c288032e') no-repeat center center/cover;
      height: 80vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      color: white;
      text-shadow: 2px 2px 6px rgba(0,0,0,0.6);
      text-align: center;
    }
    .hero h1 {
      font-size: 3rem;
      margin-bottom: 20px;
    }
    .hero button {
      padding: 12px 25px;
      border: none;
      background: #FFD700;
      color: #000;
      cursor: pointer;
      font-size: 18px;
      border-radius: 5px;
    }

    /* Menu Section */
    .menu {
      padding: 40px;
      background: #f4f4f4;
    }
    .menu h2 {
      text-align: center;
      margin-bottom: 20px;
      font-size: 2rem;
    }
    .menu-items {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .item {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      text-align: center;
    }
    .item img {
      width: 100%;
      border-radius: 10px;
      margin-bottom: 10px;
    }
    .item h3 {
      margin-bottom: 10px;
    }
    .item p {
      font-weight: bold;
      color: #8B0000;
    }

    /* About Section */
    .about {
      padding: 40px;
      text-align: center;
    }
    .about h2 {
      margin-bottom: 15px;
    }
    .about p {
      max-width: 700px;
      margin: auto;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 20px;
      background: #8B0000;
      color: #fff;
    }

    /* Responsive */
    @media(max-width: 768px) {
      nav ul {
        display: none;
        flex-direction: column;
        background: #A52A2A;
        width: 100%;
        position: absolute;
        top: 60px;
        left: 0;
      }
      nav ul.showing {
        display: flex;
      }
      .menu-toggle {
        display: block;
      }
    }
  </style>
</head>
<body>
  <!-- Navbar -->
  <nav>
    <h2>ITALIANO</h2>
    <span class="menu-toggle">☰</span>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#menu">Menu</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Hero Section -->
  <section class="hero">
    <h1>Delicious Food, Anytime!</h1>
    <p>Order your favorite meals with just one click</p>
    <button>Order Now</button>
  </section>

  <!-- Menu Section -->
  <section id="menu" class="menu">
    <h2>Our Menu</h2>
    <div class="menu-items">
      <div class="item">
        <img src="C:\Users\ashik\Downloads\istockphoto-1393150881-612x612.jpg" alt="Pizza">
        <h3>Cheese Pizza</h3>
        <p>₹899</p>
      </div>
      <div class="item">
        <img src="C:\Users\ashik\Downloads\indian-style-burger-1957599-hero-01-266103a4bb4e4ee7b5feb4da2d2e99da.jpg" alt="Burger">
        <h3>Classic Burger</h3>
        <p>560₹</p>
      </div>
      <div class="item">
        <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836" alt="Pasta">
        <h3>Italian Pasta</h3>
        <p>₹578</p>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="about">
    <h2>About Us</h2>
    <p>At ITALIANO, we believe in serving delicious, fresh, and high-quality meals. Whether you’re craving pizza, burgers, or pasta, we’ve got something for everyone. Come dine with us or order online for quick delivery!</p>
  </section>

  <!-- Footer -->
  <footer id="contact">
    <p>&copy; 2025 ITALIANO | Contact: +91 99999999999</p>
  </footer>

  <!-- JavaScript for Menu -->
  <script>
    const toggle = document.querySelector('.menu-toggle');
    const navLinks = document.querySelector('nav ul');

    toggle.addEventListener('click', () => {
      navLinks.classList.toggle('showing');
    });
  </script>
</body>
</html>
