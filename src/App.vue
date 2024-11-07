<template>
  <div>
    <nav class="navbar">
      <div class="logo">
        <img src="https://i.ibb.co/1zNvwsY/business-logo2.jpg" alt="Business Logo" style="max-width: 70%; height: auto;">
      </div>
      <button class="menu-toggle" aria-label="Toggle Menu">&#9776;</button>
      <ul class="nav-links">
        <li><a href="#" class="default-active">Home</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">About Me</a></li>
        <li><a href="#">Gallery</a></li>
        <li><a href="#">Contact Me</a></li>
      </ul>
      <button class="hire-btn" aria-label="Hire Me">Hire Me</button>
    </nav>

    <hr />

    <section class="hero">
      <div class="content-left">
        <p>Hello, I am</p>
        <h1>Gregory Wilson</h1>
        <h2>Web Front End Developer</h2>
        <h2>For Small Businesses</h2>

        <div class="social-icons">
          <a href="https://www.linkedin.com/in/greg-wilson-10a4354/" target="_blank" rel="noopener noreferrer">
            <i class="fa fa-linkedin fa-stack-3x"></i>
          </a>
          <a href="https://www.facebook.com/profile.php?id=837434234" target="_blank" rel="noopener noreferrer">
            <i class="fa fa-facebook fa-stack-3x"></i>
          </a>
        </div>
        <br />
        <div class="buttons">
          <button class="btn hire-me" aria-label="Hire Me">Hire Me</button>
        </div>
      </div>

      <div class="content-right">
        <img src="https://i.ibb.co/PQQtw3g/gw-caricature.jpg" alt="Caricature Image" class="profile-image" />
      </div>
    </section>

    <section class="info-section">
      <div class="info-box">
        <h3>5+</h3>
        <p>Experiences</p>
      </div>
      <div class="info-box">
        <h3>20+</h3>
        <p>Projects Done</p>
      </div>
      <div class="info-box">
        <h3>100+</h3>
        <p>Happy Clients</p>
      </div>
    </section>
  </div>
</template>

<script setup>
// Optional: Import FontAwesome here if it’s not globally included in your project.
// import '@fortawesome/fontawesome-free/css/all.css';
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  background-color: #000;
  color: #fff;
}

.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 15px 30px;
  background-color: #000;
  color: white;
  font-size: 1.75rem;
  position: relative;
}

.logo {
  font-size: 1.5rem;
  color: #f74d4d;
}

.menu-toggle {
  display: none;
  font-size: 1.5rem;
  background: none;
  color: white;
  border: none;
  cursor: pointer;
}

.nav-links {
  display: flex;
  list-style: none;
  gap: 20px;
}

.nav-links a {
  color: white;
  text-decoration: none;
  transition: color 0.3s ease;
}

.nav-links a.default-active {
  color: orange;
  font-weight: bold;
}

.nav-links a:hover {
  color: orange;
  font-weight: bold;
}

.hire-btn {
  background-color: #f74d4d;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.hero {
  display: flex;
  gap: 110px;
  align-items: center;
  justify-content: center;
  padding: 54px;
  color: #ccc;
  background-color: #000;
}

.content-left {
  max-width: 40%;
}

.content-left h1 {
  font-size: 2.5rem;
  margin: 10px 0;
  color: #f76d4d;
}

.content-left h2 {
  font-size: 1.8rem;
  color: orange;
}

.content-left p {
  font-size: 1.2rem;
}

.social-icons {
  display: flex;
  gap: 15px;
  margin-top: 20px;
}

.social-icons i {
  font-size: 1.5rem;
  color: #ccc;
  transition: color 0.3s ease, transform 0.3s ease;
}

.social-icons i:hover {
  color: orange;
  transform: scale(1.2);
}

.hire-me,
.btn,
.social-icons {
  transition: background-color 0.3s ease, color 0.3s ease, box-shadow 0.3s ease;
}

.hire-me:hover,
.btn:hover {
  background-color: orange;
  box-shadow: 0px 0px 10px rgba(255, 165, 0, 0.5);
}

.profile-image {
  width: 300px;
  height: auto;
  border-radius: 50%;
  object-fit: cover;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.profile-image:hover {
  transform: scale(1.05);
  box-shadow: 0px 0px 15px 5px rgba(255, 165, 0, 0.7);
}

.info-section {
  display: flex;
  justify-content: center;
  gap: 30px;
  background-color: #333;
  padding: 20px 0;
  color: #ccc;
}

.info-box {
  text-align: center;
  padding: 25px;
}

.info-box h3 {
  font-size: 1.8rem;
  color: orange;
}

.info-box p {
  color: #ccc;
}

@media (max-width: 768px) {
  .navbar {
    flex-wrap: wrap;
  }
  .menu-toggle {
    display: block;
  }
  .nav-links {
    display: none;
    flex-direction: column;
    gap: 10px;
    width: 100%;
    text-align: center;
    margin-top: 10px;
  }
  .navbar.open .nav-links {
    display: flex;
  }
  .hero {
    flex-direction: column;
    padding: 30px;
  }
  .content-left {
    max-width: 100%;
    text-align: center;
  }
  .profile-image {
    width: 200px;
  }
  .info-section {
    flex-direction: column;
    gap: 15px;
    padding: 10px 0;
  }
}
</style>
