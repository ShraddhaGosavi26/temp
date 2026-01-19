


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RestroCafe | Taste the Tradition</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="web_pg.css">
</head>
<body>
    <nav class="navbar">
        <div class="nav-container">
            <h3 id="logo">Restro<span>Cafe</span></h3>
            <ul class="links">
                <li><a href="#">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </div>
    </nav>
    <header class="hero">
        <div class="hero-content">
            <h1>Taste the Tradition</h1>
            <p>From bean to cup, we provide the finest organic coffee and handcrafted snacks in the heart of the city.</p>
            <a href="#menu" class="btn">Explore Menu</a>
        </div>
    </header>
    <section class="menu-section" id="menu">
        <div class="container">
            <h2 class="section-title">Our Popular Specials</h2>
            <div class="menu-grid">
                <div class="menu-card">
                    <div class="menu-image coffee"></div>
                    <div class="menu-info">
                        <h3>Caramel Macchiato</h3>
                        <p>Freshly steamed milk with vanilla-flavored syrup marked with espresso.</p>
                        <span class="price">$5.50</span>
                    </div>
                </div>
                <div class="menu-card">
                    <div class="menu-image toast"></div>
                    <div class="menu-info">
                        <h3>Avocado Toast</h3>
                        <p>Whole grain bread topped with smashed avocado, lime, and red pepper flakes.</p>
                        <span class="price">$12.00</span>
                    </div>
                </div>
                <div class="menu-card">
                    <div class="menu-image waffles"></div>
                    <div class="menu-info">
                        <h3>Belgian Waffles</h3>
                        <p>Crispy golden waffles served with fresh berries and maple syrup.</p>
                        <span class="price">$10.50</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <footer>
        <p>&copy; 2026 RestroCafe. Designed with ❤️ for coffee lovers.</p>
    </footer>

</body>
</html>

/* General Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary-color: #6F4E37; /* Coffee Brown */
    --accent-color: #C19A6B;  /* Camel/Latte */
    --dark-color: #2C1E16;
    --light-color: #FDF5E6;   /* Old Lace / Cream */
}

body {
    font-family: 'Poppins', sans-serif;
    line-height: 1.6;
    color: var(--dark-color);
    background-color: var(--light-color);
    scroll-behavior: smooth;
}

/* Navigation */
.navbar {
    background: white;
    padding: 1rem 5%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top: 0;
    z-index: 1000;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}

.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
}

#logo {
    font-family: 'Playfair Display', serif;
    font-size: 1.8rem;
    color: var(--primary-color);
}

#logo span {
    color: var(--accent-color);
}

.links {
    display: flex;
    list-style: none;
}

.links li {
    margin-left: 2rem;
}

.links a {
    text-decoration: none;
    color: var(--dark-color);
    font-weight: 600;
    transition: 0.3s;
}

.links a:hover {
    color: var(--primary-color);
}

/* Hero Section */
.hero {
    height: 80vh;
    background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), 
                url('https://images.unsplash.com/photo-1495474472287-4d71bcdd2085?auto=format&fit=crop&q=80&w=2070');
    background-size: cover;
    background-position: center;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: white;
}

.hero-content h1 {
    font-family: 'Playfair Display', serif;
    font-size: 4rem;
    margin-bottom: 1rem;
}

.hero-content p {
    font-size: 1.2rem;
    max-width: 600px;
    margin: 0 auto 2rem;
}

.btn {
    display: inline-block;
    padding: 1rem 2.5rem;
    background-color: var(--primary-color);
    color: white;
    text-decoration: none;
    border-radius: 50px;
    font-weight: bold;
    transition: 0.3s;
}

.btn:hover {
    background-color: var(--accent-color);
    transform: translateY(-3px);
}

/* Menu Section */
.menu-section {
    padding: 5rem 10%;
    max-width: 1200px;
    margin: 0 auto;
}

.section-title {
    text-align: center;
    font-family: 'Playfair Display', serif;
    font-size: 2.5rem;
    margin-bottom: 3rem;
    position: relative;
}

.section-title::after {
    content: '';
    display: block;
    width: 80px;
    height: 3px;
    background: var(--accent-color);
    margin: 10px auto;
}

.menu-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
}

.menu-card {
    background: white;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
    transition: 0.3s;
}

.menu-card:hover {
    transform: scale(1.03);
}

.menu-image {
    height: 200px;
    background-size: cover;
    background-position: center;
}

/* Specific item images */
.coffee { background-image: url('https://images.unsplash.com/photo-1541167760496-162955ed8a9f?q=80&w=500'); }
.toast { background-image: url('https://images.unsplash.com/photo-1525351484163-7529414344d8?q=80&w=500'); }
.waffles { background-image: url('https://images.unsplash.com/photo-1562329265-95a6d7a83440?q=80&w=500'); }

.menu-info {
    padding: 1.5rem;
}

.menu-info h3 {
    margin-bottom: 0.5rem;
}

.menu-info p {
    font-size: 0.9rem;
    color: #666;
    margin-bottom: 1rem;
}

.price {
    font-weight: bold;
    color: var(--primary-color);
    font-size: 1.2rem;
}

/* Footer */
footer {
    background-color: var(--dark-color);
    color: white;
    text-align: center;
    padding: 2rem;
    margin-top: 3rem;
}

/* Responsive */
@media (max-width: 768px) {
    .links { display: none; } /* Simplified for this example */
    .hero-content h1 { font-size: 2.5rem; }
}
