<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Essentique - Luxury Perfumes</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Raleway:wght@300;400;700&display=swap" rel="stylesheet">
    
    <style>
        /* CSS styles are embedded directly here for a single-file setup */
        
        /* Base Styles */
        body {
            font-family: 'Raleway', sans-serif; 
            margin: 0;
            padding: 0;
            background-color: #0d0d0d; /* Deep charcoal black background */
            color: #e0e0e0; /* Light gray for body text */
            direction: ltr; 
            text-align: left;
            line-height: 1.6;
        }

        h1, h2, h3 {
            font-family: 'Playfair Display', serif; /* Elegant serif for headings */
            color: #ffd700; /* Gold for headings */
            text-align: center;
            margin-bottom: 20px;
        }

        h1 { font-size: 2.8em; }
        h2 { font-size: 2.2em; }
        h3 { font-size: 1.6em; }

        /* Header & Navigation */
        header {
            background-color: #1a1a1a; 
            color: #ffd700; 
            padding: 15px 50px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5); 
            border-bottom: 1px solid #333; 
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .header-logo {
            width: 60px; 
            height: auto;
            margin-right: 15px;
            filter: drop-shadow(0 0 5px rgba(255, 215, 0, 0.4)); 
        }

        header h1 {
            margin: 0;
            font-size: 2.2em;
            letter-spacing: 2px;
            text-align: left;
        }

        header nav a {
            color: #ffd700; 
            text-decoration: none;
            margin-left: 30px;
            font-weight: 400; 
            font-family: 'Raleway', sans-serif;
            letter-spacing: 1px;
            transition: color 0.3s, text-shadow 0.3s;
        }

        header nav a:hover {
            color: #fff; 
            text-shadow: 0 0 8px rgba(255, 215, 0, 0.7); 
        }

        /* Main Content Area */
        main {
            padding: 50px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        main h2 {
            color: #ffd700;
            margin-bottom: 40px;
            position: relative;
            padding-bottom: 15px;
        }

        main h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 2px;
            background-color: #ffd700; 
        }

        /* Perfume Grid Layout */
        .perfume-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); 
            gap: 40px;
            padding: 20px 0;
        }

        /* Perfume Card Design */
        .perfume-card {
            background-color: #1a1a1a; 
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.6); 
            transition: transform 0.4s ease-in-out, box-shadow 0.4s ease-in-out;
            text-align: center;
            padding: 25px;
            border: 1px solid #333; 
        }

        .perfume-card:hover {
            transform: translateY(-8px) scale(1.02); 
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.8);
            border-color: #ffd700; 
        }

        .perfume-card img {
            width: 100%;
            max-height: 300px; 
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 20px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3); 
        }

        .perfume-card h3 {
            color: #ffd700; 
            margin-bottom: 10px;
            font-size: 1.8em;
            letter-spacing: 1px;
        }

        .perfume-card .description {
            font-size: 1em;
            color: #b0b0b0; 
            min-height: 60px; 
            overflow: hidden;
            margin-bottom: 20px;
        }

        .perfume-card .price {
            font-size: 1.5em;
            color: #ffd700; 
            font-weight: 700;
            margin: 15px 0;
            letter-spacing: 1px;
        }

        /* Add to Cart Button */
        .add-to-cart {
            background-color: #ffd700; 
            color: #1a1a1a; 
            border: none;
            padding: 12px 28px;
            border-radius: 30px;
            cursor: pointer;
            font-weight: 700;
            font-family: 'Raleway', sans-serif;
            font-size: 1.1em;
            letter-spacing: 1px;
            transition: background-color 0.3s, transform 0.3s;
        }

        .add-to-cart:hover {
            background-color: #ffc107; 
            transform: translateY(-2px);
        }

        /* About Section */
        .about-section {
            background-color: #1a1a1a;
            padding: 60px 20px;
            margin: 60px auto;
            max-width: 1000px;
            border-radius: 12px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.6);
            text-align: center;
            border: 1px solid #333;
        }

        .about-section h2 {
            color: #ffd700;
            margin-bottom: 30px;
        }

        .about-section p {
            font-size: 1.1em;
            color: #e0e0e0;
            margin-bottom: 20px;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        /* Footer */
        footer {
            background-color: #1a1a1a;
            color: #b0b0b0;
            text-align: center;
            padding: 30px 0;
            margin-top: 60px;
            border-top: 1px solid #333;
        }

        footer p {
            margin: 5px 0;
        }

        footer a {
            color: #ffd700;
            text-decoration: none;
            transition: color 0.3s;
        }

        footer a:hover {
            color: #fff;
            text-decoration: underline;
        }

        .social-links img {
            width: 28px;
            height: 28px;
            margin: 0 8px;
            filter: drop-shadow(0 0 3px rgba(255, 215, 0, 0.3));
            transition: transform 0.3s;
        }

        .social-links img:hover {
            transform: scale(1.1);
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">
            <img src="images/essentique_logo.png" alt="Essentique Logo" class="header-logo"> 
            <h1>Essentique</h1>
        </div>
        <nav>
            <a href="#products">Fragrances</a>
            <a href="#about">About Us</a>
            <a href="#contact">Contact</a>
            <a href="#cart">🛒 Cart</a>
        </nav>
    </header>

    <main id="products">
        <h2>Discover Our Exquisite Collection</h2>
        
        <section class="perfume-grid">
            
            <div class="perfume-card">
                <img src="images/perfume1.jpg" alt="Mystic Oud Perfume">
                <h3>Mystic Oud Elixir</h3>
                <p class="description">A captivating blend of deep oud and delicate jasmine, a scent that truly lingers.</p>
                <p class="price">**Price:** $120</p>
                <button class="add-to-cart">Add to Cart</button>
            </div>

            <div class="perfume-card">
                <img src="images/perfume2.jpg" alt="Summer Breeze Perfume">
                <h3>Golden Hour Bloom</h3>
                <p class="description">Fresh citrus notes with a hint of rose, perfect for an uplifting daily wear.</p>
                <p class="price">**Price:** $95</p>
                <button class="add-to-cart">Add to Cart</button>
            </div>

            <div class="perfume-card">
                <img src="images/perfume3.jpg" alt="Enchanted Forest Perfume">
                <h3>Whispering Woods</h3>
                <p class="description">Earthy patchouli and cedarwood mingle with subtle spices for a truly unique aroma.</p>
                <p class="price">**Price:** $110</p>
                <button class="add-to-cart">Add to Cart</button>
            </div>
            
        </section>
    </main>
    
    <section id="about" class="about-section">
        <h2>The Essentique Story</h2>
        <p>At Essentique, we believe that fragrance is an art form. Each bottle encapsulates a journey, a memory, a feeling. Handcrafted with the finest ingredients, our perfumes are designed to evoke emotion and leave an unforgettable impression. Discover the essence of luxury.</p>
        <p>Our commitment to quality ensures that every spritz is a moment of pure indulgence.</p>
    </section>
</head>
</html>
