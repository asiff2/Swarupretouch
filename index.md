<html lang="en">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Swarup Retouch | AI Fashion Visualization Studio</title>
<meta name="description" content="AI-powered fashion visualization studio transforming flat lay apparel into premium AI model visuals for modern brands.">

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>

/* ---------------- THEME SYSTEM ---------------- */

:root {
    --bg:#0f172a;
    --surface:rgba(255,255,255,0.06);
    --text:#f8fafc;
    --muted:#94a3b8;
    --primary:#6366f1;
    --accent:#06b6d4;
}

.light-mode {
    --bg:#f9fbff;
    --surface:#ffffff;
    --text:#111827;
    --muted:#6b7280;
}

body {
    margin:0;
    font-family:'Inter',sans-serif;
    background:var(--bg);
    color:var(--text);
    transition:0.3s ease;
    overflow-x:hidden;
}

/* ---------------- ANIMATED GRADIENT MESH ---------------- */

.mesh {
    position:fixed;
    width:100%;
    height:100%;
    background: radial-gradient(circle at 20% 30%, rgba(99,102,241,0.3), transparent 40%),
                radial-gradient(circle at 80% 70%, rgba(6,182,212,0.3), transparent 40%);
    animation: moveMesh 15s infinite alternate ease-in-out;
    z-index:-1;
}

@keyframes moveMesh {
    0% { transform:translate(0,0) scale(1); }
    100% { transform:translate(-50px,-50px) scale(1.1); }
}

/* ---------------- NAV ---------------- */

nav {
    display:flex;
    justify-content:space-between;
    padding:20px 40px;
    backdrop-filter:blur(10px);
}

nav ul {
    display:flex;
    list-style:none;
    gap:30px;
}

nav a {
    text-decoration:none;
    color:var(--text);
}

/* ---------------- BUTTON ---------------- */

.btn {
    padding:12px 28px;
    border-radius:8px;
    background:linear-gradient(90deg,var(--primary),var(--accent));
    color:white;
    text-decoration:none;
    display:inline-block;
}

/* ---------------- HERO ---------------- */

.hero {
    text-align:center;
    padding:140px 20px 80px;
}

.hero h1 {
    font-size:56px;
}

/* ---------------- 3D FLOATING MOCKUP ---------------- */

.mockup-container {
    perspective:1200px;
    display:flex;
    justify-content:center;
    margin-top:60px;
}

.mockup {
    width:400px;
    height:400px;
    border-radius:20px;
    overflow:hidden;
    box-shadow:0 40px 80px rgba(0,0,0,0.4);
    animation: float 6s ease-in-out infinite;
    transform-style:preserve-3d;
}
.mockup img {
    width:100%;
    height:100%;
    object-fit:cover;
    border-radius:20px;
}
@keyframes float {
    0% { transform:rotateY(-15deg) rotateX(5deg) translateY(0); }
    50% { transform:rotateY(15deg) rotateX(-5deg) translateY(-20px); }
    100% { transform:rotateY(-15deg) rotateX(5deg) translateY(0); }
}

/* ---------------- SECTIONS ---------------- */

section {
    max-width:1100px;
    margin:auto;
    padding:100px 20px;
}

/* ---------------- CLIENTS TESTIMONIALS & RATINGS ---------------- */

.grid {
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:40px;
}

.card {
    background:var(--surface);
    padding:40px;
    border-radius:20px;
}

/* ---------------- BLOG ---------------- */

.blog-card h3 {
    margin-bottom:10px;
}

/* ---------------- CONTACT FORM ---------------- */

form {
    max-width:500px;
    margin:auto;
    display:flex;
    flex-direction:column;
    gap:15px;
}

input, textarea {
    padding:12px;
    border-radius:8px;
    border:none;
    font-family:inherit;
}

footer {
    text-align:center;
    padding:60px 20px;
    color:var(--muted);
}

.toggle {
    cursor:pointer;
    padding:6px 12px;
    border:1px solid var(--text);
    border-radius:20px;
}

</style>
</head>

<body>

<div class="mesh"></div>

<nav>
    <strong>Swarup Retouch</strong>
    <ul>
        <li><a href="#cases">Client Testimonials</a></li>
        <li><a href="blog.html">Blog</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><span class="toggle" onclick="toggleMode()">Toggle Mode</span></li>
    </ul>
</nav>

<section class="hero">
    <h1>AI Fashion Visualization <br> For Modern Brands</h1>
    <p>Launch collections 80% faster with premium AI model imagery.</p>
    <br>
    <a href="#contact" class="btn">Start Project</a>

    <div class="mockup-container">
        <div class="mockup">
        <img src="images/model1.jpg" alt="AI Fashion Model 1">
        </div>
    </div>
</section>

<section id="cases">
    <h2>Case Studies</h2>
    <div class="grid">
        <div class="card">
            <h3>Luxury Ethnic Brand</h3>
            <p>Reduced photoshoot costs by 75% while scaling 50+ SKUs.</p>
            <a href="case-study-1.html">submit your testimonials & Ratings →</a>
        </div>
        <div class="card">
            <h3>D2C Streetwear Startup</h3>
            <p>Launched full lookbook in 48 hours.</p>
            <a href="case-study-2.html">Read Case Study →</a>
        </div>
    </div>
</section>

<section>
    <h2>From Our Blog</h2>
    <div class="grid">
        <div class="card blog-card">
            <h3>How AI Is Replacing Fashion Photoshoots</h3>
            <p>Why modern brands are switching to AI-generated models.</p>
            <a href="blog.html">Read More →</a>
        </div>
        <div class="card blog-card">
            <h3>Cost Breakdown: Traditional vs AI Shoots</h3>
            <p>A data-driven comparison for apparel brands.</p>
            <a href="blog.html">Read More →</a>
        </div>
    </div>
</section>

<section id="contact">
    <h2>Start Your Project</h2>

    <!-- CRM READY (Replace action with HubSpot/Zoho webhook if needed) -->
    <form action="https://formspree.io/f/maqdzbal" method="POST">
        <input type="text" name="name" placeholder="Your Name" required>
        <input type="email" name="email" placeholder="Your Email" required>
        <textarea name="message" rows="4" placeholder="Tell us about your social media handles"></textarea>
        <button class="btn" type="submit">Submit</button>
    </form>
</section>

<footer>
© 2026 Swarup Retouch | AI Fashion Visualization Studio
</footer>

<script>

/* DARK MODE TOGGLE */
function toggleMode(){
    document.body.classList.toggle("light-mode");
    localStorage.setItem("mode",
        document.body.classList.contains("light-mode") ? "light" : "dark"
    );
}

if(localStorage.getItem("mode")==="light"){
    document.body.classList.add("light-mode");
}

</script>

</body>
</html>
