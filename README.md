
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мой сайт на GitHub</title>
    <style>
        /* Общие стили */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Шапка */
        header {
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            color: white;
            padding: 80px 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="%23ffffff" fill-opacity="0.1" d="M0,96L48,112C96,128,192,160,288,186.7C384,213,480,235,576,213.3C672,192,768,128,864,128C960,128,1056,192,1152,192C1248,192,1344,128,1392,96L1440,64L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>');
            background-size: cover;
            background-position: center;
        }
        
        .header-content {
            position: relative;
            z-index: 1;
        }
        
        h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
        }
        
        .subtitle {
            font-size: 1.5rem;
            margin-bottom: 30px;
            opacity: 0.9;
        }
        
        .btn {
            display: inline-block;
            background-color: #ff7e5f;
            color: white;
            padding: 12px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        }
        
        .btn:hover {
            background-color: #ff9a8b;
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0,0,0,0.25);
        }
        
        /* Основной контент */
        section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            font-size: 2.5rem;
            color: #2c3e50;
        }
        
        .features {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 30px;
        }
        
        .feature {
            flex: 1;
            min-width: 300px;
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }
        
        .feature:hover {
            transform: translateY(-10px);
        }
        
        .feature-icon {
            font-size: 3rem;
            margin-bottom: 20px;
            color: #6a11cb;
        }
        
        .feature h3 {
            margin-bottom: 15px;
            color: #2c3e50;
        }
        
        /* Галерея */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .gallery-item {
            height: 250px;
            border-radius: 10px;
            overflow: hidden;
            position: relative;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .gallery-item:hover img {
            transform: scale(1.1);
        }
        
        /* Контактная форма */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
        }
        
        input, textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
        
        textarea {
            min-height: 150px;
            resize: vertical;
        }
        
        /* Подвал */
        footer {
            background-color: #2c3e50;
            color: white;
            padding: 40px 0;
            text-align: center;
        }
        
        .social-links {
            margin: 20px 0;
        }
        
        .social-links a {
            display: inline-block;
            margin: 0 10px;
            color: white;
            font-size: 1.5rem;
            transition: color 0.3s ease;
        }
        
        .social-links a:hover {
            color: #6a11cb;
        }
        
        /* Адаптивность */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            .subtitle {
                font-size: 1.2rem;
            }
            
            .features {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <!-- Шапка -->
    <header>
        <div class="container">
            <div class="header-content">
                <h1>Добро пожаловать на мой сайт</h1>
                <p class="subtitle">Создан с любовью для GitHub Pages</p>
                <a href="#about" class="btn">Узнать больше</a>
            </div>
        </div>
    </header>

    <!-- О сайте -->
    <section id="about">
        <div class="container">
            <h2 class="section-title">О сайте</h2>
            <div class="features">
                <div class="feature">
                    <div class="feature-icon">🚀</div>
                    <h3>Современный дизайн</h3>
                    <p>Этот сайт создан с использованием современных технологий HTML5 и CSS3, что обеспечивает отличный внешний вид и удобство использования.</p>
                </div>
                <div class="feature">
                    <div class="feature-icon">📱</div>
                    <h3>Адаптивный</h3>
                    <p>Сайт отлично выглядит на всех устройствах - от смартфонов до настольных компьютеров благодаря адаптивному дизайну.</p>
                </div>
                <div class="feature">
                    <div class="feature-icon">⚡</div>
                    <h3>Быстрая загрузка</h3>
                    <p>Оптимизированный код обеспечивает быструю загрузку страницы, что улучшает пользовательский опыт и SEO.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Галерея -->
    <section style="background-color: #f0f4f8;">
        <div class="container">
            <h2 class="section-title">Галерея</h2>
            <div class="gallery">
                <div class="gallery-item">
                    <img src="https://picsum.photos/400/300?random=1" alt="Изображение 1">
                </div>
                <div class="gallery-item">
                    <img src="https://picsum.photos/400/300?random=2" alt="Изображение 2">
                </div>
                <div class="gallery-item">
                    <img src="https://picsum.photos/400/300?random=3" alt="Изображение 3">
                </div>
                <div class="gallery-item">
                    <img src="https://picsum.photos/400/300?random=4" alt="Изображение 4">
                </div>
                <div class="gallery-item">
                    <img src="https://picsum.photos/400/300?random=5" alt="Изображение 5">
                </div>
                <div class="gallery-item">
                    <img src="https://picsum.photos/400/300?random=6" alt="Изображение 6">
                </div>
            </div>
        </div>
    </section>

    <!-- Контакты -->
    <section id="contact">
        <div class="container">
            <h2 class="section-title">Свяжитесь со мной</h2>
            <div class="contact-form">
                <form>
                    <div class="form-group">
                        <label for="name">Имя</label>
                        <input type="text" id="name" placeholder="Ваше имя">
                    </div>
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" placeholder="Ваш email">
                    </div>
                    <div class="form-group">
                        <label for="message">Сообщение</label>
                        <textarea id="message" placeholder="Ваше сообщение"></textarea>
                    </div>
                    <button type="submit" class="btn">Отправить</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Подвал -->
    <footer>
        <div class="container">
            <p>© 2023 Мой сайт на GitHub Pages. Все права защищены.</p>
            <div class="social-links">
                <a href="#">GitHub</a>
                <a href="#">Twitter</a>
                <a href="#">LinkedIn</a>
                <a href="#">Instagram</a>
            </div>
        </div>
    </footer>
</body>
</html>
