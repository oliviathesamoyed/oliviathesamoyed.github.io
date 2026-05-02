```
style.css

```
  
/* --- OLIVIA BRAND VARIABLES --- */  
:root {  
    --crimson: #D62828;  
    --white: #FFFFFF;  
    --nyc-stone: #F9F9F9;  
    --charcoal: #2B2D42;  
    --font-heading: 'Playfair Display', serif;  
    --font-body: 'Montserrat', sans-serif;  
}  
  
/* --- GLOBAL STYLES --- */  
* {  
    margin: 0;  
    padding: 0;  
    box-sizing: border-box;  
}  
  
body {  
    font-family: var(--font-body);  
    color: var(--charcoal);  
    line-height: 1.7;  
    background-color: var(--white);  
    -webkit-font-smoothing: antialiased;  
}  
  
h1, h2, h3 {  
    font-family: var(--font-heading);  
    margin-bottom: 20px;  
    font-weight: 600;  
}  
  
p {  
    margin-bottom: 20px;  
    font-size: 1.05rem;  
}  
  
/* --- REUSABLE CLASSES --- */  
.container {  
    max-width: 1100px;  
    margin: 0 auto;  
    padding: 0 20px;  
}  
  
.section {  
    padding: 100px 0;  
}  
  
.bg-stone { background-color: var(--nyc-stone); }  
.bg-dark { background-color: var(--charcoal); }  
.text-white { color: var(--white); }  
.text-center { text-align: center; }  
.max-width-800 { max-width: 800px; margin: 0 auto; }  
  
.label {  
    display: block;  
    color: var(--crimson);  
    font-size: 0.85rem;  
    font-weight: 600;  
    letter-spacing: 2px;  
    margin-bottom: 10px;  
}  
  
.heart-icon-large {  
    color: var(--crimson);  
    font-size: 3rem;  
    line-height: 1;  
    margin-bottom: 20px;  
}  
  
/* --- NAVIGATION --- */  
nav {  
    background-color: rgba(255, 255, 255, 0.98);  
    position: fixed;  
    width: 100%;  
    top: 0;  
    z-index: 100;  
    border-bottom: 1px solid #EAEAEA;  
    padding: 20px 0;  
}  
  
.nav-container {  
    display: flex;  
    justify-content: space-between;  
    align-items: center;  
    max-width: 1200px;  
    margin: 0 auto;  
    padding: 0 30px;  
}  
  
.logo {  
    font-weight: 600;  
    letter-spacing: 3px;  
    font-size: 1.1rem;  
}  
  
.nav-links {  
    list-style: none;  
    display: flex;  
    align-items: center;  
    gap: 30px;  
}  
  
.nav-links a {  
    text-decoration: none;  
    color: var(--charcoal);  
    font-size: 0.85rem;  
    text-transform: uppercase;  
    letter-spacing: 1px;  
    transition: color 0.3s ease;  
}  
  
.nav-links a:hover { color: var(--crimson); }  
  
.cta-small {  
    background-color: var(--crimson);  
    color: var(--white) !important;  
    padding: 10px 20px;  
    border-radius: 30px;  
}  
  
/* --- HERO SECTION --- */  
.hero {  
    height: 100vh;  
    display: flex;  
    align-items: center;  
    justify-content: center;  
    text-align: center;  
    background-color: var(--nyc-stone);  
    /* LATER: You will add Olivia's photo here */  
    padding: 0 20px;  
    margin-top: 50px;  
}  
  
.brand-line {  
    font-size: 3.5rem;  
    font-style: italic;  
    max-width: 900px;  
    margin: 0 auto 20px;  
    line-height: 1.2;  
}  
  
.sub-headline {  
    font-size: 1.2rem;  
    letter-spacing: 1px;  
    color: #555;  
}  
  
/* --- GRID LAYOUT (For Books/Westminster) --- */  
.grid {  
    display: grid;  
    grid-template-columns: 1fr 1fr;  
    gap: 60px;  
    align-items: center;  
}  
  
.image-box {  
    background-color: #E0E0E0;  
    height: 450px;  
    border-radius: 8px;  
    display: flex;  
    align-items: center;  
    justify-content: center;  
    color: #777;  
    font-size: 0.9rem;  
    letter-spacing: 1px;  
}  
  
.book-quote {  
    border-left: 3px solid var(--crimson);  
    padding-left: 20px;  
    font-style: italic;  
    font-family: var(--font-heading);  
    font-size: 1.3rem;  
    margin: 30px 0;  
    color: #555;  
}  
  
/* --- BUTTONS --- */  
.btn-primary {  
    display: inline-block;  
    background-color: var(--crimson);  
    color: var(--white);  
    padding: 15px 40px;  
    text-decoration: none;  
    border-radius: 50px;  
    font-weight: 600;  
    margin-top: 20px;  
    letter-spacing: 1px;  
    transition: transform 0.3s ease;  
}  
  
.btn-primary:hover {  
    transform: translateY(-3px);  
}  
  
/* --- FOOTER --- */  
footer {  
    padding: 40px 0;  
    background-color: var(--white);  
    border-top: 1px solid #EAEAEA;  
    font-size: 0.9rem;  
}  
  
.legal-text {  
    font-size: 0.75rem;  
    color: #888;  
    margin-bottom: 15px;  
}  
  
.socials a {  
    color: var(--charcoal);  
    text-decoration: none;  
    margin: 0 10px;  
    font-weight: 600;  
}  
  
/* --- MOBILE RESPONSIVENESS --- */  
@media (max-width: 768px) {  
    .nav-links { display: none; } /* Hide links on tiny screens for now */  
    .brand-line { font-size: 2.2rem; }  
    .grid { grid-template-columns: 1fr; }  
    .grid.reverse .image-box { grid-row: 1; } /* Keeps image on top on mobile */  
}  
