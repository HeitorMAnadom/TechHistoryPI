# HEADER DEFINITIVO

<-- css DESKTOP -->
html{
padding-top: 7vw;
}

div.desktop {
    display: block;
  }

  header {
    display: flex;
    background-color: #000000af;
    font-size: 0.4rem;
    padding: 0.5vw;
    position: fixed;
    top: 0vw;
    z-index: 10;
    width: 100%;
  }

  header a img {
    height: 5vw;
    padding: 0vw 2vw;
  }

  header a.quiz-button {
    background-color: #1f1d3a;
    padding: 1.2vw;
    border-radius: 2vw;
  }

  header a.quiz-button:hover {
    background: none;
    border: solid 1px white;
    transition: ease 1s;
  }

  header div.desktop nav {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }

  .desktop ul {
    display: flex;
    gap: 2vw;
    position: fixed;
    right: 3vw;
  }

  .menu {
    display: none;
  }

<--css MOBILE-->

header {
  color: white;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

header img {
  height: 15vw;
}

.menu {
  font-size: 30px;
  background: none;
  border: none;
  cursor: pointer;
  padding: 15px;
}

.sidebar {
  position: fixed;
  top: 0;
  left: 0;
  width: 175px;
  height: 120%;
  background-image: linear-gradient(to right, #000000, #1f1d3adc);
  padding-top: 60px;
  z-index: 10;
  transform: translateX(-100%);
  transition: transform 0.3s ease-in-out;
  font-size: 15px;
  border-right: solid 2px rgb(2, 87, 59);
  border-radius: 10px;
}

.sidebar.open {
  transform: translateX(0);
  backdrop-filter: blur(10px);
}

.sidebar ul li a {
  padding: 15px 25px;
  text-decoration: none;
  font-size: 18px;
  color: #ffffff;
  display: block;
  transition: 0.2s;
}

.sidebar a:hover {
  color: #f1f1f1;
  background-color: #222;
}

.sidebar .close-btn {
  position: absolute;
  top: 10px;
  right: 25px;
  font-size: 36px;
  background: none;
  border: none;
  color: #ffffff;
  cursor: pointer;
}

.overlay {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 5;
}

.overlay.open {
  display: block;
}

<-- HTML -->

 <header>
      <div class="desktop">
        <nav>
          <a href=""><img src="Pagina_1/source/logo_cortada.png" alt="" /></a>
          <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="Pagina_1/sobre.html">Sobre</a></li>
            <li><a href="Pagina_2/evolucao.html">Evolução</a></li>
            <li><a href="Pagina_3/circulacao.html">Circulação</a></li>
            <li><a href="Pagina_4/impactos.html">Impactos</a></li>
            <li><a href="Pagina_5/costumes.html">Curiosidades</a></li>
            <li><a href="Pagina_6/antiguidades.html">Antiguidades</a></li>
            <li>
              <a class="quiz-button" href="Quiz/index.html">Jogue Quiz!</a>
            </li>
          </ul>
        </nav>
      </div>
      <div class="menuzao">
        <button class="menu" onclick="toggleMenu()">&#9776;</button>
        <nav class="sidebar" id="sidebar">
          <button class="close-btn" onclick="toggleMenu()">&times;</button>
          <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="Pagina_1/sobre.html">Sobre</a></li>
            <li><a href="Pagina_2/evolucao.html">Evolução</a></li>
            <li><a href="Pagina_3/circulacao.html">Circulação</a></li>
            <li><a href="Pagina_4/impactos.html">Impactos</a></li>
            <li><a href="Pagina_5/costumes.html">Curiosidades</a></li>
            <li><a href="Pagina_6/antiguidades.html">Antiguidades</a></li>
            <li><a href="Quiz/index.html">Jogue Quiz!</a></li>
          </ul>
        </nav>
        <div class="overlay" id="overlay" onclick="toggleMenu()"></div>
        <script>
          function toggleMenu() {
            const sidebar = document.getElementById("sidebar");
            const overlay = document.getElementById("overlay");
            sidebar.classList.toggle("open");
            overlay.classList.toggle("open");
          }
        </script>
      </div>
      <img class="mobile" src="Pagina_1/source/logo_cortada.png" alt="" />
    </header>


  
  img.mobile {
    display: none;
  }
