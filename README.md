# PRODIGY_WD_01
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Responsive Landing Page</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
    }

    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background-color: #ba5a5a;
      z-index: 1000;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
    }

    nav ul {
      list-style: none;
      display: flex;
      justify-content: center;
      padding: 1em 0;
    }

    nav ul li {
      margin: 0 15px;
    }

    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      padding: 8px 12px;
      border-radius: 4px;
      transition: all 0.3s ease;
    }

    /* Unique hover colors */
    nav ul li:nth-child(1) a:hover {
      background-color: #ff6f61;
      color: white;
    }

    nav ul li:nth-child(2) a:hover {
      background-color: #1e90ff;
      color: white;
    }

    nav ul li:nth-child(3) a:hover {
      background-color: #32cd32;
      color: white;
    }

    nav ul li:nth-child(4) a:hover {
      background-color: #ff1493;
      color: white;
    }

    section {
      padding: 100px 20px;
      min-height: 100vh;
    }

    #home {
      background: orchid;
    }

    #features {
      background: palegreen;
    }

    #about {
      background: rebeccapurple;
      color: white;
    }

    #contact {
      background: yellowgreen;
    }

    h1, h2 {
      margin-bottom: 20px;
    }

    p {
      font-size: 1.1rem;
    }
  </style>
</head>
<body>

  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#features">Features</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <section id="home">
    <h1>Welcome to the Landing Page</h1>
    <p>This is a responsive and interactive landing page.</p>
  </section>

  <section id="features">
    <h2>Features</h2>
    <p>Some cool features go here.</p>
  </section>

  <section id="about">
    <h2>About</h2>
    <p>Information about us.</p>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <p>Get in touch with us.</p>
  </section>

  <script>
    // Optional: Highlight nav item on scroll (basic)
    const sections = document.querySelectorAll("section");
    const navLinks = document.querySelectorAll("nav ul li a");

    window.addEventListener("scroll", () => {
      let current = "";
      sections.forEach(section => {
        const sectionTop = section.offsetTop - 100;
        if (pageYOffset >= sectionTop) {
          current = section.getAttribute("id");
        }
      });

      navLinks.forEach(link => {
        link.classList.remove("active");
        if (link.getAttribute("href") === #${current}) {
          link.classList.add("active");
        }
      });
    });
  </script>
</body>
</html>
