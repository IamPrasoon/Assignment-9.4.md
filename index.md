
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>CodeWithPrasoon</title>
<style>
* { box-sizing: border-box; }
body {
    margin: 0;
    font-family: Arial, sans-serif;
    color: #222;
}
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 8%;
    background: #142d60;
    color: white;
}
nav { display: flex; gap: 25px; }
nav a { color: white; text-decoration: none; }

.hero {
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    gap: 40px;
    padding: 70px 8%;
    background: #eaf3ff;
}
.hero h1 { font-size: 42px; }
.hero p { line-height: 1.6; }
.hero img { width: 100%; max-width: 450px; }

.btn {
    display: inline-block;
    background: #ff9800;
    color: black;
    padding: 12px 25px;
    border-radius: 5px;
    text-decoration: none;
}
.features { padding: 50px 8%; text-align: center; }
.cards {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 20px;
}
.card {
    background: #f2f2f2;
    padding: 30px;
    border-radius: 10px;
}
footer {
    background: #142d60;
    color: white;
    text-align: center;
    padding: 20px;
}
@media (max-width: 700px) {
    header { flex-wrap: wrap; gap: 15px; }
    nav { flex-wrap: wrap; }
    .hero, .cards { grid-template-columns: 1fr; }
    .hero { padding: 30px 8%; }
    .hero h1 { font-size: 30px; }
}
</style>
</head>
<body>

<header>
    <h2>CodeWithPrasoon</h2>
    <nav>
        <a href="#home">Home</a>
        <a href="#features">Features</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<main>
    <section class="hero" id="home">
        <div>
            <h1>Learn Web Development</h1>
            <p>Master HTML, CSS and JavaScript
            to build modern websites.</p>
            <a class="btn" href="#features">Get Started</a>
        </div>
        <img src="images/coding.jpg" alt="Coding illustration">
    </section>

    <section class="features" id="features">
        <h2>Our Features</h2>
        <div class="cards">
            <article class="card">
                <h3>HTML</h3>
                <p>Learn website structure.</p>
            </article>
            <article class="card">
                <h3>CSS</h3>
                <p>Create beautiful designs.</p>
            </article>
            <article class="card">
                <h3>JavaScript</h3>
                <p>Build interactive websites.</p>
            </article>
        </div>
    </section>
</main>

<footer id="contact">
    <p>&copy; 2026 Prasoon Anand</p>
</footer>

</body>
</html>
