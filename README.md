<!DOCTYPE html>
<html lang="fr">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="style.css">
  <title>Mini-site</title>
</head>

<body>

  <h1>Mon mini-site</h1>

  <p class="intro">
    Ceci est une page d’entraînement pour pratiquer le lien CSS, les class, les id et la notion parent/enfant.
  </p>

  <h2>Menu</h2>
  <ul id="menu">
    <li><a class="nav-link" href="#">Accueil</a></li>
    <li><a class="nav-link" href="#">Services</a></li>
    <li><a class="nav-link" href="#">Contact</a></li>
  </ul>

  <h2>Présentation</h2>
  <div id="card">
    <p id="important">
      Ce paragraphe est spécial : on veut le styler différemment des autres.
    </p>

    <p>
      Ce paragraphe est normal mais il est dans la carte.
      On veut le différencier des paragraphes situés en dehors de la carte.
    </p>

    <a class="highlight" href="#">Voir plus</a>
  </div>

  <p>
    Ce paragraphe est en dehors de la carte.
    Il ne doit pas avoir le même style que les paragraphes dans la carte.
  </p>

  <img src="img/image.jpg" alt="Image de démonstration">

</body>

</html>

html {
  background-color: black;
  color: white;
  font-family: Arial, sans-serif;
}

h1 {
  color: grey;
  font-size: 60px;
}

h2 {
  color: #cfcfcf;
  font-size: 28px;
}

a {
  color: red;
  text-decoration: none;
}

.nav-link {
  color: white;
  font-weight: bold;
}

#card {
  background-color: red;
  border-radius: 10px;
  width: 300px;
  padding: 20px;
  margin: 25px;
}

#card p {
  color: black;
  margin: 10px 0;
}

#card p#important {
  margin: 0;
  color: black;
  font-weight: bold;
}

.highlight {
  background-color: black;
  color: white;
  padding: 8px 12px;
  border-radius: 8px;
}
formulaire 
<!DOCTYPE html>
<html lang="fr">

<head>
    <meta charset="UTF-8">
    <title>Titre de la page</title>
</head>

<body>

    <!-- ========================= -->
    <!-- HEADER : En-tête du site -->
    <!-- ========================= -->
    <header>
        <h1>Titre principal</h1>
        <p>Introduction courte</p>
    </header>

    <!-- ========================= -->
    <!-- MAIN : Contenu principal -->
    <!-- ========================= -->
    <main>

        <section>
            <h2>Premier bloc</h2>

            <form action="#" method="get">
                <!-- Champs du premier formulaire -->
            </form>
        </section>

        <section>
            <h2>Deuxième bloc</h2>

            <form action="#" method="post">
                <!-- Champs du second formulaire -->
            </form>
        </section>

    </main>

    <!-- ========================= -->
    <!-- FOOTER : Pied de page -->
    <!-- ========================= -->
    <footer>
        <p>Pied de page</p>
    </footer>

</body>

</html>

flexbox
<hr>

<h2>TP2</h2>

<section id="tp2">

    <h3>Display</h3>
    <div class="display-zone">
        <div class="box">BOX 1</div>
        <div class="box">BOX 2</div>
        <div class="box">BOX 3</div>
    </div>

    <h3>Position</h3>
    <div class="promo-card">
        <p class="promo-title">Offre spéciale</p>
        <p>Le badge doit être placé dans le coin en haut à droite.</p>
        <span class="badge">NEW</span>
    </div>

    <h3>Flexbox</h3>
    <div class="services">
        <div class="service-card">
            <h4>Service 1</h4>
            <p>Texte simple.</p>
        </div>

        <div class="service-card">
            <h4>Service 2</h4>
            <p>Texte simple.</p>
        </div>

        <div class="service-card">
            <h4>Service 3</h4>
            <p>Texte simple.</p>
        </div>
    </div>

</section>


