<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RideNow | Accueil - Stages Moto</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>

    <header>
        <nav class="navbar">
            <div class="logo">Ride<span>Now</span></div>
            <ul class="nav-links">
                <li><a href="index.html" class="active">Accueil</a></li>
                <li><a href="stages.html">Nos Stages</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <h1>Dominez la route avec RideNow</h1>
            <p>Des coachings personnalisés pour tous les niveaux, du débutant au pistard confirmé.</p>
            <a href="stages.html" class="btn">Découvrir nos stages</a>
        </section>

        <section class="intro">
            <h2>Pourquoi choisir RideNow ?</h2>
            <p>Notre centre propose des expériences uniques pour améliorer votre sécurité et votre plaisir de conduite.</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 RideNow - Centre de perfectionnement moto. Tous droits réservés.</p>
    </footer>

</body>
</html>



------
style.css
/* Reset & Base */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
}

/* Header & Nav */
header {
    background: #1a1a1a;
    color: #fff;
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 1000;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 20px;
}

.logo {
    font-size: 1.5rem;
    font-weight: bold;
    text-transform: uppercase;
}

.logo span { color: #e74c3c; }

.nav-links {
    display: flex;
    list-style: none;
}

.nav-links li a {
    color: #fff;
    text-decoration: none;
    margin-left: 20px;
    transition: color 0.3s;
}

.nav-links li a:hover, .nav-links li a.active {
    color: #e74c3c;
}

/* Hero Section */
.hero {
    background: #2c3e50;
    color: white;
    height: 60vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 20px;
}

.btn {
    display: inline-block;
    background: #e74c3c;
    color: white;
    padding: 10px 25px;
    text-decoration: none;
    margin-top: 20px;
    border-radius: 5px;
}

/* Footer */
footer {
    background: #1a1a1a;
    color: white;
    text-align: center;
    padding: 2rem 0;
    margin-top: 50px;
}

----stage html 
/* Grille de stages */
.stages-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    max-width: 1100px;
    margin: 40px auto;
    padding: 0 20px;
}

.stage-card {
    border: 1px solid #ddd;
    border-radius: 8px;
    overflow: hidden;
    flex: 1 1 calc(33.333% - 20px); /* 3 colonnes par défaut */
    display: flex;
    flex-direction: column;
}

.stage-card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.stage-content { padding: 15px; }


---- fin fichier css
/* Tablette */
@media (max-width: 900px) {
    .stage-card {
        flex: 1 1 calc(50% - 20px); /* 2 colonnes */
    }
}

/* Mobile */
@media (max-width: 600px) {
    .navbar {
        flex-direction: column;
    }
    
    .nav-links {
        margin-top: 15px;
    }

    .stage-card {
        flex: 1 1 100%; /* 1 seule colonne */
    }
    
    .hero h1 { font-size: 1.5rem; }
}


