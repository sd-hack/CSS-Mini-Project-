# CSS-Mini-Project-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mini Landing Page</title>

<style>
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
}

/* ---------- HEADER ---------- */
header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 40px;
  background: #0d6efd;
  color: white;
}

.logo{
  font-size: 22px;
  font-weight: bold;
}

nav a{
  color: white;
  margin-left: 20px;
  text-decoration: none;
  transition: 0.3s;
}

nav a:hover{
  text-decoration: underline;
  color: #ffd700;
}

/* ---------- HERO SECTION ---------- */
.hero{
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
  padding: 60px 40px;
  background: #f5f7ff;
  align-items: center;
}

.hero-text h1{
  font-size: 40px;
  margin-bottom: 15px;
}

.hero-text p{
  font-size: 16px;
  margin-bottom: 20px;
  color: #444;
}

.hero-text button{
  padding: 12px 25px;
  border: none;
  background: #0d6efd;
  color: white;
  border-radius: 6px;
  cursor: pointer;
  transition: 0.3s;
}

.hero-text button:hover{
  background: #084298;
  transform: scale(1.05);
}

.hero img{
  width: 100%;
  max-width: 400px;
}

/* ---------- FEATURES ---------- */
.features{
  padding: 60px 40px;
  background: white;
  text-align: center;
}

.features h2{
  margin-bottom: 40px;
}

.cards{
  display: flex;
  gap: 20px;
  justify-content: center;
}

.card{
  background: #f2f2f2;
  padding: 25px;
  width: 250px;
  border-radius: 10px;
  transition: 0.3s;
}

.card:hover{
  transform: translateY(-10px);
  background: #e0e7ff;
}

.card h3{
  margin: 15px 0 10px;
}

/* ---------- FOOTER ---------- */
footer{
  background: #0d6efd;
  color: white;
  text-align: center;
  padding: 20px;
}

footer a{
  color: white;
  margin: 0 10px;
  text-decoration: none;
}

footer a:hover{
  text-decoration: underline;
}

/* ---------- RESPONSIVE ---------- */
@media(max-width: 768px){

  header{
    flex-direction: column;
    gap: 10px;
  }

  .hero{
    grid-template-columns: 1fr;
    text-align: center;
  }

  .cards{
    flex-direction: column;
    align-items: center;
  }

  .hero-text h1{
    font-size: 28px;
  }
}
</style>
</head>

<body>

<!-- HEADER -->
<header>
  <div class="logo">SkillTech</div>
  <nav>
    <a href="#">Home</a>
    <a href="#">Features</a>
    <a href="#">Contact</a>
  </nav>
</header>

<!-- HERO -->
<section class="hero">
  <div class="hero-text">
    <h1>Build Your Future with Coding</h1>
    <p>Learn web development and create beautiful websites using HTML and CSS.</p>
    <button>Get Started</button>
  </div>

  <img src="https://cdn-icons-png.flaticon.com/512/1055/1055687.png" alt="coding">
</section>

<!-- FEATURES -->
<section class="features">
  <h2>Our Features</h2>

  <div class="cards">
    <div class="card">
      <h3>Easy Learning</h3>
      <p>Simple tutorials to start coding quickly.</p>
    </div>

    <div class="card">
      <h3>Responsive Design</h3>
      <p>Websites that look great on all devices.</p>
    </div>

    <div class="card">
      <h3>Career Ready</h3>
      <p>Skills that companies really want.</p>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <p>© 2026 SkillTech. All rights reserved.</p>
  <p>
    <a href="#">Facebook</a> |
    <a href="#">Instagram</a> |
    <a href="#">LinkedIn</a>
  </p>
</footer>

</body>
</html>
