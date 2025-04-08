EStoy creando una web para mi server de sam, ahi te mando la estructura 
public/
index.html
informacion.html
tienda.html
css/
style.css
js/
scripts.js
imgs/
background.jpg
logo.png


index.html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Servidor GTA San Multiplayer</title>
    <link rel="stylesheet" href="../css/style.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap" rel="stylesheet">
</head>
<body>
    <header>
        <nav class="navbar">
            <ul class="menu">
                <li><a href="index.html">INICIO</a></li>
                <li><a href="tienda.html">TIENDA</a></li>
                <li><a href="informacion.html">INFORMACIÓN</a></li>
                <li><a href="https://discord.gg/9nD3Wmph9q" class="discord-btn">DISCORD</a></li>
            </ul>
        </nav>
    </header>
    <div class="hero">
        <div class="content">
            <h1>El mejor servidor de GTA San Multiplayer</h1>
            <p>Explora un mundo único lleno de aventuras y rol.</p>
            <div class="buttons">
                <a href="#" class="button play">JUGAR AHORA</a>
                <a href="#" class="button guide">VER GUÍA</a>
            </div>
        </div>
        <div class="server-info">
            <img src="../imgs/logo.png" alt="Logo Servidor GTA San Multiplayer">
        </div>
    </div>
    <div class="ip-box">
        <p>IP: 92.133.12.78:7777</p>
    </div>
</body>
</html>

informacion.html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Información</title>
    <link rel="stylesheet" href="../css/style.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap" rel="stylesheet">
</head>
<body>
    <header>
        <nav class="navbar">
            <ul class="menu">
                <li><a href="index.html">INICIO</a></li>
                <li><a href="tienda.html">TIENDA</a></li>
                <li><a href="informacion.html">INFORMACIÓN</a></li>
                <li><a href="https://discord.gg/9nD3Wmph9q" class="discord-btn">DISCORD</a></li>
            </ul>
        </nav>
    </header>
    <main class="content">
        <h1>Información</h1>
        <p>Descubre más sobre nuestro servidor y únete a una comunidad de jugadores apasionados.</p>
    </main>
</body>
</html>

tiends.html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tienda</title>
    <link rel="stylesheet" href="../css/style.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap" rel="stylesheet">
</head>
<body>
    <header>
        <nav class="navbar">
            <ul class="menu">
                <li><a href="index.html">INICIO</a></li>
                <li><a href="tienda.html">TIENDA</a></li>
                <li><a href="informacion.html">INFORMACIÓN</a></li>
                <li><a href="https://discord.gg/9nD3Wmph9q" class="discord-btn">DISCORD</a></li>
            </ul>
        </nav>
    </header>
    <main class="content">
        <h1>Tienda</h1>
        <p>Aquí puedes adquirir todo lo que necesitas para mejorar tu experiencia en GTA San Multiplayer.</p>
    </main>
</body>
</html>

scripts.js
......

style.css
/* General */
body, html {
    margin: 0;
    padding: 0;
    height: 100%;
    font-family: 'Poppins', sans-serif;
    color: white;
    background-color: black;
}

/* Navbar */
header {
    background: rgba(0, 0, 0, 0.8);
    padding: 1rem 2rem;
    position: fixed;
    width: 100%;
    display: flex;
    justify-content: start;
    align-items: center;
    z-index: 10;
}

.menu {
    list-style: none;
    display: flex;
    gap: 1.5rem;
    margin: 0;
    padding: 0;
}

.menu li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s ease;
}

.menu li a:hover {
    color: #5a00ff;
}

/* Botón Discord */
.discord-btn {
    background-color: #5a00ff;
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
    transition: background-color 0.3s ease, transform 0.3s ease;
}

.discord-btn:hover {
    background-color: #4500cc;
    transform: scale(1.1);
}

/* Hero Section */
.hero {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100vh;
    padding: 2rem;
    background: url('../imgs/background.jpg') no-repeat center center/cover;
    position: relative;
}

.hero::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.6);
    backdrop-filter: blur(10px);
    z-index: 1;
}

.content {
    position: relative;
    z-index: 2;
    max-width: 50%;
}

.content h1 {
    font-size: 3.5rem;
    font-weight: 600;
    margin-bottom: 1rem;
}

.content p {
    font-size: 1.5rem;
    margin-bottom: 2rem;
}

.buttons {
    display: flex;
    gap: 1rem;
}

.button {
    text-decoration: none;
    padding: 1rem 2rem;
    border-radius: 30px;
    font-size: 1rem;
    font-weight: 600;
    transition: all 0.3s ease;
}

.button.play {
    background-color: #5a00ff;
    color: white;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.2);
}

.button.play:hover {
    background-color: #4500cc;
    transform: scale(1.1);
}

.button.guide {
    background-color: transparent;
    border: 2px solid #5a00ff;
    color: #5a00ff;
}

.button.guide:hover {
    background-color: #5a00ff;
    color: white;
    transform: scale(1.1);
}

/* Server Info */
.server-info {
    position: relative;
    z-index: 2;
    text-align: right;
    max-width: 50%;
}

.server-info img {
    width: 300px;
}

/* IP Box */
.ip-box {
    position: absolute;
    bottom: 5%;
    left: 50%;
    transform: translateX(-50%);
    background-color: #000000cc;
    padding: 1rem 2rem;
    border-radius: 10px;
    border: 2px solid #5a00ff;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.3);
    z-index: 3;
}

.ip-box p {
    font-size: 1.5rem;
    font-weight: bold;
    color: #5a00ff;
    margin: 0;
    text-align: center;
}