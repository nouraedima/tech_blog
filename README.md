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


<section class="stages-section">
    <h2 style="text-align: center; margin-top: 30px;">Nos Expériences Moto</h2>
    
    <div class="stages-container">
        <article class="stage-card">
            <img src="img/maniabilite.jpg" alt="Moto maniabilité">
            <div class="stage-content">
                <h3>Maniabilité & Équilibre</h3>
                <p>Maîtrisez votre moto à basse vitesse : demi-tours, évitements et freinages d'urgence pour plus de sécurité au quotidien.</p>
                <p><strong>Durée :</strong> 1 journée</p>
            </div>
        </article>

        <article class="stage-card">
            <img src="img/piste.jpg" alt="Moto sur piste">
            <div class="stage-content">
                <h3>Initiation Piste</h3>
                <p>Découvrez les trajectoires et la position de conduite sur circuit sécurisé avec nos coachs diplômés d'État.</p>
                <p><strong>Durée :</strong> 2 jours</p>
            </div>
        </article>

        <article class="stage-card">
            <img src="img/voyage.jpg" alt="Moto route">
            <div class="stage-content">
                <h3>Perfectionnement Route</h3>
                <p>Améliorez votre lecture de trajectoire en virage et gagnez en confiance lors de vos sorties en groupe.</p>
                <p><strong>Durée :</strong> 1/2 journée</p>
            </div>
        </article>
    </div>
</section>


<section class="contact-container">
    <h2>Contactez RideNow</h2>
    <p>Une question sur nos tarifs ou nos disponibilités ? Écrivez-nous.</p>

    <form class="contact-form">
        <div class="form-group">
            <label for="nom">Nom complet</label>
            <input type="text" id="nom" name="nom" required placeholder="Votre nom">
        </div>

        <div class="form-group">
            <label for="email">Email</label>
            <input type="email" id="email" name="email" required placeholder="votre@email.com">
        </div>

        <div class="form-group">
            <label for="stage">Stage souhaité</label>
            <select id="stage" name="stage">
                <option value="maniabilite">Maniabilité</option>
                <option value="piste">Piste</option>
                <option value="route">Route</option>
            </select>
        </div>

        <div class="form-group">
            <label for="message">Message</label>
            <textarea id="message" name="message" rows="5" required></textarea>
        </div>

        <button type="submit" class="btn">Envoyer la demande</button>
    </form>
</section>


