<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chemodany.kg | Рюкзаки и Чемоданы</title>
    <style>
        /* CSS Styles */
        :root {
            --primary-color: #2c3e50;
            --accent-color: #27ae60;
            --bg-color: #f8f9fa;
            --text-color: #333;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
        }

        /* Header */
        header {
            background-color: white;
            padding: 20px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: var(--primary-color);
            text-decoration: none;
        }

        .nav-links a {
            margin-left: 20px;
            text-decoration: none;
            color: var(--primary-color);
            font-weight: 500;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 80px 20px;
            background: linear-gradient(rgba(44, 62, 80, 0.8), rgba(44, 62, 80, 0.8)), url('https://images.unsplash.com/photo-1553062407-98eeb64c6a62?ixlib=rb-1.2.1&auto=format&fit=crop&w=1950&q=80') center/cover;
            color: white;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 15px;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
        }

        /* Product Grid */
        .container {
            max-width: 1200px;
            margin: 50px auto;
            padding: 0 20px;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
            font-size: 2rem;
            color: var(--primary-color);
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .product-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }

        .product-card:hover {
            transform: translateY(-5px);
        }

        .product-image {
            width: 100%;
            height: 300px;
            object-fit: cover;
        }

        .product-info {
            padding: 20px;
            text-align: center;
        }

        .product-title {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: var(--primary-color);
        }

        .product-price {
            font-size: 1.4rem;
            font-weight: bold;
            color: var(--primary-color);
            margin-bottom: 15px;
        }

        .buy-btn {
            background-color: var(--accent-color);
            color: white;
            border: none;
            padding: 10px 25px;
            border-radius: 25px;
            font-size: 1rem;
            cursor: pointer;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 8px;
            transition: background-color 0.3s;
            text-decoration: none;
        }

        .buy-btn:hover {
            background-color: #219a52;
        }

        /* Footer */
        footer {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 40px 20px;
            margin-top: 50px;
        }

        .social-links {
            margin-top: 15px;
        }

        .social-links a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        /* Mobile Adjustments */
        @media (max-width: 768px) {
            .nav-links {
                display: none; /* Can be replaced with a hamburger menu later */
            }
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <a href="#" class="logo">CHEMODANY.KG</a>
        <nav class="nav-links">
            <a href="#catalog">Каталог</a>
            <a href="#contact">Контакты</a>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <h1>Стильные рюкзаки и чемоданы</h1>
        <p>Надежные спутники для ваших путешествий и городских будней</p>
    </section>

    <!-- Catalog Section -->
    <div class="container" id="catalog">
        <h2 class="section-title">Хиты продаж</h2>
        
        <div class="product-grid">
            <!-- Product 1 -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1553062407-98eeb64c6a62?auto=format&fit=crop&w=500&q=80" alt="Рюкзак Urban Explorer" class="product-image">
                <div class="product-info">
                    <h3 class="product-title">Рюкзак Urban Explorer</h3>
                    <div class="product-price">2 500 сом</div>
                    <!-- Replace 996555123456 with your actual WhatsApp number -->
                    <button class="buy-btn" onclick="orderViaWhatsApp('Рюкзак Urban Explorer', '2 500 сом', '996555123456')">
                        Купить через WhatsApp
                    </button>
                </div>
            </div>

            <!-- Product 2 -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1491013516836-7dbf43681048?auto=format&fit=crop&w=500&q=80" alt="Дорожный рюкзак Travel Pro" class="product-image">
                <div class="product-info">
                    <h3 class="product-title">Дорожный рюкзак Travel Pro</h3>
                    <div class="product-price">3 200 сом</div>
                    <button class="buy-btn" onclick="orderViaWhatsApp('Дорожный рюкзак Travel Pro', '3 200 сом', '996555123456')">
                        Купить через WhatsApp
                    </button>
                </div>
            </div>

            <!-- Product 3 -->
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1598532163257-ae3c6b2524b6?auto=format&fit=crop&w=500&q=80" alt="Городской чемодан" class="product-image">
                <div class="product-info">
                    <h3 class="product-title">Компактный чемодан S-size</h3>
                    <div class="product-price">4 500 сом</div>
                    <button class="buy-btn" onclick="orderViaWhatsApp('Компактный чемодан S-size', '4 500 сом', '996555123456')">
                        Купить через WhatsApp
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer id="contact">
        <h3>Магазин Chemodany.kg</h3>
        <p>г. Бишкек</p>
        <div class="social-links">
            <p>Следите за нами в Instagram: <a href="https://instagram.com/chemodany.kg" target="_blank">@chemodany.kg</a></p>
        </div>
    </footer>

    <!-- JavaScript for WhatsApp routing -->
    <script>
        function orderViaWhatsApp(productName, price, phoneNumber) {
            // Formats the message
            const message = `Здравствуйте! Хочу заказать товар с сайта chemodany.kg:%0A%0A📦 Товар: ${productName}%0A💵 Цена: ${price}%0A%0AВ наличии?`;
            
            // Redirects to WhatsApp
            const whatsappUrl = `https://wa.me/${phoneNumber}?text=${message}`;
            window.open(whatsappUrl, '_blank');
        }
    </script>
</body>
</html>
