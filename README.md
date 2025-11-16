<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Interstellar – A Complete Deep Dive</title>

<style>
/* ---------------- GLOBAL STYLE ---------------- */
:root {
    --bg: #f4f7fc;
    --card: #ffffff;
    --text: #0d0d0d;         /* PURE DARK TEXT */
    --muted: #1a1a1a;        /* DARKER MUTED - STILL DARK */
    --accent: #1b3de7;       /* Darker blue */
    --accent2: #27408b;      /* Deep navy blue */
    --radius: 16px;
    --pad: 22px;
    --shadow: 0 10px 35px rgba(0,0,0,0.09);
}

body.dark {
    --bg: #0e1117;
    --card: #151921;
    --text: #f7f7f7;         /* LIGHT TEXT FOR DARK MODE */
    --muted: #e1e1e1;        /* STILL LIGHT */
    --accent: #5f89ff;
    --accent2: #96b0ff;
    --shadow: 0 10px 40px rgba(0,0,0,0.4);
}

body {
    background: var(--bg);
    margin: 0;
    font-family: "Inter", sans-serif;
    color: var(--text);
    line-height: 1.7;
    padding-bottom: 40px;
    transition: 0.3s ease-in-out;
}

/* ---------------- LAYOUT ---------------- */
.container {
    max-width: 960px;
    margin: auto;
    padding: 20px;
}

/* ---------------- HEADER ---------------- */
header {
    background: linear-gradient(135deg, #375dfb, #6e8cff, #9bb4ff);
    padding: 40px;
    border-radius: var(--radius);
    color: #ffffff;
    box-shadow: var(--shadow);
    animation: fadeIn 0.8s ease-in-out;
}

header h1 {
    margin: 0;
    font-size: 34px;
    font-weight: 700;
}

header p {
    margin-top: 10px;
    font-size: 16px;
    opacity: 0.95;
    color: #ffffff;
}

/* ---------------- DARK MODE BUTTON ---------------- */
.toggle-btn {
    position: fixed;
    right: 20px;
    top: 20px;
    background: var(--accent);
    color: #fff;
    border: none;
    padding: 10px 16px;
    font-size: 14px;
    border-radius: 50px;
    cursor: pointer;
    box-shadow: var(--shadow);
    transition: 0.2s;
}
.toggle-btn:hover {
    transform: scale(1.05);
}

/* ---------------- TABLE OF CONTENTS ---------------- */
.toc {
    background: var(--card);
    padding: 20px;
    border-radius: var(--radius);
    margin: 25px 0;
    box-shadow: var(--shadow);
}

.toc h3 {
    margin-top: 0;
    color: var(--accent);
}

.toc a {
    display: block;
    padding: 6px 0;
    text-decoration: none;
    color: var(--accent);
}
.toc a:hover {
    color: var(--text);
}

/* ---------------- ARTICLE ---------------- */
article {
    background: var(--card);
    padding: var(--pad);
    border-radius: var(--radius);
    box-shadow: var(--shadow);
    animation: fadeIn 1s ease;
}

h2 {
    margin-top: 26px;
    color: var(--accent);
}

h3 {
    margin-top: 14px;
    color: var(--accent2);
}

p, li {
    color: var(--text);   /* TEXT ALWAYS DARK */
}

ul {
    margin-left: 22px;
}

/* ---------------- ANIMATIONS ---------------- */
@keyframes fadeIn {
    from { opacity: 0; transform: translateY(15px); }
    to { opacity: 1; transform: translateY(0); }
}

</style>
</head>

<body>

<button class="toggle-btn" onclick="document.body.classList.toggle('dark')">
🌙 / ☀️
</button>

<div class="container">

<header>
    <h1>Interstellar: Why Christopher Nolan’s Space Epic Still Dominates Modern Sci-Fi</h1>
    <p>A complete deep dive into the film’s science, storytelling, themes, visuals, and emotional depth.</p>
</header>

<div class="toc">
    <h3>Table of Contents</h3>
    <a href="#intro">Introduction</a>
    <a href="#world">1. The World of Interstellar</a>
    <a href="#mission">2. The Mission</a>
    <a href="#planets">3. The Planets</a>
    <a href="#miller">— Miller’s Planet</a>
    <a href="#mann">— Mann’s Planet</a>
    <a href="#edmund">— Edmund’s Planet</a>
    <a href="#science">4. The Science</a>
    <a href="#accurate">— Accurate Realism</a>
    <a href="#break">— Scientific Breakdowns</a>
    <a href="#emotional">5. Emotional Core</a>
    <a href="#tesseract">6. The Tesseract</a>
    <a href="#themes">7. Themes</a>
    <a href="#visuals">8. Visual Brilliance</a>
    <a href="#music">9. Music</a>
    <a href="#matters">10. Why It Still Matters</a>
    <a href="#final">Final Verdict</a>
</div>

<article>

<section id="intro">
<h2>Introduction</h2>
<p>Few sci-fi films aim high. Even fewer hit the target. Christopher Nolan’s Interstellar combines physics, emotion, philosophy, and large-scale storytelling into a single narrative. Its ambition is exactly why it still stands out today.</p>
<p>This article dives into every element of the film—science, visuals, themes, strengths, flaws, and legacy.</p>
</section>

<section id="world">
<h2>1. The World of Interstellar</h2>
<p>Earth is dying—crops failing, dust storms taking over, and hope shrinking. Humanity isn’t battling aliens; it’s battling nature and time itself.</p>
</section>

<section id="mission">
<h2>2. The Mission</h2>
<p>Cooper and NASA scientists travel through a wormhole to find a new habitable world. The wormhole visuals are guided by Kip Thorne’s real physics calculations.</p>
</section>

<section id="planets">
<h2>3. The Planets</h2>
<p>Three candidate worlds—each symbolizing a different fate for humanity.</p>
</section>

<section id="miller">
<h3>Miller’s Planet — The Cost of Time</h3>
<p>Near Gargantua, time stretches: 1 hour = 7 years on Earth. The emotional hit of decades lost is heavier than the giant waves.</p>
</section>

<section id="mann">
<h3>Mann’s Planet — Desperation</h3>
<p>Dr. Mann represents fear taken to an extreme, almost destroying the mission.</p>
</section>

<section id="edmund">
<h3>Edmund’s Planet — Hope</h3>
<p>The final planet offers a real chance for humanity’s survival.</p>
</section>

<section id="science">
<h2>4. The Science</h2>
<p>Interstellar pushes harder than most sci-fi films to stay scientifically grounded.</p>
</section>

<section id="accurate">
<h3>Accurate or Realistic Elements</h3>
<ul>
<li>Time dilation near a massive black hole</li>
<li>Relativity and gravitational effects</li>
<li>Wormhole representation based on real math</li>
<li>Black hole imagery used in academic research</li>
<li>Space-time interactions affecting the plot</li>
</ul>
</section>

<section id="break">
<h3>Where It Breaks Down</h3>
<ul>
<li>The tesseract scene bends scientific rules</li>
<li>“Love is a dimension” is poetic, not scientific</li>
<li>Surviving a black hole is unlikely</li>
</ul>
</section>

<section id="emotional">
<h2>5. Emotional Core</h2>
<p>The father–daughter relationship between Cooper and Murph drives the emotional narrative of the film.</p>
</section>

<section id="tesseract">
<h2>6. The Tesseract</h2>
<p>A visually stunning but scientifically debatable moment where the story shifts from physics to metaphysics.</p>
</section>

<section id="themes">
<h2>7. Themes</h2>
<ul>
<li>Time as an enemy</li>
<li>Sacrifice</li>
<li>Human resilience</li>
<li>Exploration as survival</li>
</ul>
</section>

<section id="visuals">
<h2>8. Visual Brilliance</h2>
<p>Nolan’s practical effects and accurate black hole rendering set a new standard in sci-fi visuals.</p>
</section>

<section id="music">
<h2>9. Music</h2>
<p>Hans Zimmer’s organ-driven score delivers emotional and atmospheric impact.</p>
</section>

<section id="matters">
<h2>10. Why Interstellar Still Matters</h2>
<p>The film blends scientific ambition with emotional and philosophical storytelling.</p>
</section>

<section id="final">
<h2>Final Verdict</h2>
<p>Interstellar remains one of the boldest sci-fi films ever made—ambitious, emotional, visually stunning, and scientifically daring.</p>
</section>

</article>

</div>

<script>
document.querySelector(".toggle-btn").addEventListener("click", () => {
    document.body.classList.toggle("dark");
});
</script>

</body>
</html>
