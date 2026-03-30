# LoLHub
A site for all the LoL fans
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Arcane Nexus — League Hub</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
:root {
  --deep-navy: #0A0F1F;
  --violet-shadow: #1C1038;
  --arcane-blue: #3AB4F2;
  --neon-teal: #00E5C0;
  --magenta-glow: #C94BDB;
  --soft-gray: #D9D9D9;
  --off-white: #F5F5F5;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Inter', sans-serif;
  background: linear-gradient(135deg, var(--deep-navy), var(--violet-shadow));
  color: var(--soft-gray);
}

/* NAVBAR */
nav {
  display: flex;
  justify-content: space-between;
  padding: 20px 40px;
  background: rgba(10,15,31,0.9);
  position: sticky;
  top: 0;
}

nav h1 {
  color: var(--neon-teal);
}

nav ul {
  display: flex;
  gap: 25px;
  list-style: none;
}

nav a {
  color: var(--soft-gray);
  text-decoration: none;
  position: relative;
}

nav a:hover {
  color: var(--arcane-blue);
}

nav a::after {
  content: "";
  position: absolute;
  bottom: -5px;
  left: 0;
  width: 0%;
  height: 2px;
  background: var(--neon-teal);
  transition: 0.3s;
}

nav a:hover::after {
  width: 100%;
}

/* HERO */
.hero {
  text-align: center;
  padding: 120px 20px;
}

.hero h2 {
  font-size: 48px;
  color: var(--off-white);
}

.hero p {
  margin-top: 10px;
  font-size: 18px;
}

.buttons {
  margin-top: 30px;
}

.btn {
  padding: 12px 25px;
  margin: 10px;
  border-radius: 8px;
  border: none;
  cursor: pointer;
  font-weight: bold;
}

.btn-primary {
  background: var(--neon-teal);
  color: var(--deep-navy);
}

.btn-primary:hover {
  background: var(--arcane-blue);
  box-shadow: 0 0 12px var(--arcane-blue);
}

.btn-secondary {
  background: transparent;
  border: 2px solid var(--arcane-blue);
  color: var(--arcane-blue);
}

/* CARDS */
.section {
  padding: 60px 40px;
}

.cards {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
}

.card {
  flex: 1;
  min-width: 280px;
  background: rgba(28,16,56,0.85);
  padding: 25px;
  border-radius: 12px;
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 0 15px var(--arcane-blue);
}

.highlight {
  border: 1px solid var(--magenta-glow);
  box-shadow: 0 0 12px rgba(201,75,219,0.4);
}

h3 {
  color: var(--off-white);
  margin-bottom: 10px;
}

/* CHAMPIONS */
.champions {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
  gap: 20px;
}

.champion {
  background: rgba(28,16,56,0.85);
  padding: 15px;
  border-radius: 10px;
  text-align: center;
  transition: 0.3s;
}

.champion:hover {
  box-shadow: 0 0 10px var(--neon-teal);
}

/* FOOTER */
footer {
  text-align: center;
  padding: 30px;
  margin-top: 40px;
  background: rgba(10,15,31,0.8);
}
</style>
</head>

<body>

<!-- NAV -->
<nav>
  <h1>Arcane Nexus</h1>
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">New Players</a></li>
    <li><a href="#">Advanced</a></li>
    <li><a href="#">Champions</a></li>
    <li><a href="#">Meta Builds</a></li>
  </ul>
</nav>

<!-- HERO -->
<section class="hero">
  <h2>Master the Rift</h2>
  <p>From your first game to Challenger</p>

  <div class="buttons">
    <button class="btn btn-primary">Start Learning</button>
    <button class="btn btn-secondary">Explore Meta</button>
  </div>
</section>

<!-- PATHS -->
<section class="section">
  <div class="cards">

    <div class="card">
      <h3>New Players</h3>
      <p>Learn roles, map awareness, and beginner champions.</p>
      <button class="btn btn-primary">Start Journey</button>
    </div>

    <div class="card highlight">
      <h3>Advanced Players</h3>
      <p>Master macro, wave control, and climb faster.</p>
      <button class="btn btn-primary">Climb Faster</button>
    </div>

  </div>
</section>

<!-- GUIDES -->
<section class="section">
  <h3>Guides</h3>
  <div class="cards">

    <div class="card">
      <h3>Roles Explained</h3>
      <p>Top, Jungle, Mid, ADC, Support breakdown.</p>
    </div>

    <div class="card">
      <h3>Map Awareness</h3>
      <p>Learn vision control and rotations.</p>
    </div>

    <div class="card">
      <h3>Macro Play</h3>
      <p>Win games with smarter decisions.</p>
    </div>

  </div>
</section>

<!-- CHAMPIONS -->
<section class="section">
  <h3>Popular Champions</h3>
  <div class="champions">

    <div class="champion">Ahri</div>
    <div class="champion">Yasuo</div>
    <div class="champion">Lux</div>
    <div class="champion">Zed</div>
    <div class="champion">Jinx</div>

  </div>
</section>

<!-- META -->
<section class="section">
  <h3>Meta Builds</h3>
  <div class="cards">

    <div class="card highlight">
      <h3>Ahri Mid</h3>
      <p>Win Rate: 52%</p>
    </div>

    <div class="card highlight">
      <h3>Lee Sin Jungle</h3>
      <p>Win Rate: 49%</p>
    </div>

  </div>
</section>

<footer>
  <p>© 2026 Arcane Nexus — League Hub</p>
</footer>

<script>
// simple scroll effect
document.querySelectorAll('.btn').forEach(btn => {
  btn.addEventListener('click', () => {
    alert("Feature coming soon!");
  });
});
</script>

</body>
</html>
```
