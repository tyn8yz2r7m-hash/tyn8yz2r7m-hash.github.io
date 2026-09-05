# tyn8yz2r7m-hash.github.io
My site
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Везет КГ — Кованые прицепы для машин и квадроциклов</title>
    
    <!-- Подключение "Старославянских" шрифтов -->
    <link href="https://fonts.googleapis.com/css2?family=Ruslan+Display&family=Rubik:wght@400;600&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --gold: #d4af37;
            --dark-bg: #1a1210;
            --wood-dark: #2b1d16;
            --wood-light: #4a3324;
            --metal: #3b3f45;
            --rust: #8b3a3a;
            --text-main: #e0d6c3;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Rubik', sans-serif;
            background-color: var(--dark-bg);
            color: var(--text-main);
            background-image: 
                radial-gradient(circle at 20% 50%, rgba(139, 58, 58, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 80% 30%, rgba(212, 175, 55, 0.1) 0%, transparent 50%),
                repeating-linear-gradient(45deg, #1f1712 0px, #1f1712 2px, #241a14 2px, #241a14 4px);
            min-height: 100vh;
        }

        /* Кнопки */
        .btn {
            display: inline-block;
            padding: 12px 25px;
            background: linear-gradient(180deg, #5a3d2b, #3b261a);
            color: var(--gold);
            text-transform: uppercase;
            letter-spacing: 2px;
            font-weight: bold;
            border: 2px solid var(--gold);
            cursor: pointer;
            text-decoration: none;
            font-family: 'Rubik', sans-serif;
            transition: 0.3s;
            box-shadow: 0 4px 10px rgba(0,0,0,0.6);
            position: relative;
        }
        .btn:hover {
            background: linear-gradient(180deg, #7a5238, #4a3020);
            box-shadow: 0 0 15px rgba(212, 175, 55, 0.6);
            transform: translateY(-2px);
        }

        /* Шапка */
        header {
            background: linear-gradient(180deg, #0f0a08 0%, #211510 100%);
            border-bottom: 3px solid var(--gold);
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 5px 20px rgba(0,0,0,0.8);
        }
        .header-inner {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        .logo h1 {
            font-family: 'Ruslan Display', cursive;
            font-size: 2.2rem;
            color: var(--gold);
            text-shadow: 3px 3px 0px #000;
            letter-spacing: 3px;
            line-height: 1;
        }
        .logo p {
            font-size: 0.7rem;
            letter-spacing: 5px;
            text-transform: uppercase;
            color: #a08c6a;
        }
        nav a {
            color: var(--text-main);
            text-decoration: none;
            margin-left: 25px;
            font-weight: 600;
            text-transform: uppercase;
            font-size: 0.9rem;
            border-bottom: 1px solid transparent;
            transition: 0.3s;
        }
        nav a:hover {
            color: var(--gold);
            border-bottom: 1px solid var(--gold);
        }

        /* Герой-блок */
        .hero {
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" opacity="0.05"><path d="M0 50 L100 50 M50 0 L50 100" stroke="gold" stroke-width="2"/><circle cx="50" cy="50" r="40" stroke="gold" stroke-width="1" fill="none"/></svg>');
            background-color: #1a1210;
            padding: 60px 20px;
            text-align: center;
            border-bottom: 4px solid var(--rust);
            position: relative;

1
14:42
animation: fadeIn 1s ease-in;
        }
        .hero h2 {
            font-family: 'Ruslan Display', cursive;
            font-size: 3.5rem;
            color: #fff;
            text-shadow: 4px 4px 0px #000;
            margin-bottom: 15px;
        }
        .hero h2 span {
            color: var(--gold);
        }
        .hero p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto 30px auto;
            color: #cbb89d;
        }
        .divider {
            font-size: 2rem;
            color: var(--gold);
            letter-spacing: 15px;
            margin: 20px 0;
        }

        /* Секции */
        .section-title {
            text-align: center;
            font-family: 'Ruslan Display', cursive;
            font-size: 2rem;
            color: var(--gold);
            margin: 40px 0 20px 0;
            text-transform: uppercase;
        }

        /* Сетка карточек */
        .catalog-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        .card {
            background: linear-gradient(145deg, #2b1d16, #1a1210);
            border: 2px solid #4a3324;
            border-radius: 8px;
            overflow: hidden;
            transition: 0.4s;
            display: flex;
            flex-direction: column;
            box-shadow: 0 10px 20px rgba(0,0,0,0.5);
        }
        .card:hover {
            border-color: var(--gold);
            box-shadow: 0 0 25px rgba(212, 175, 55, 0.3);
            transform: scale(1.02);
        }
        .card-img {
            height: 200px;
            background-color: #3b3f45;
            display: flex;
            align-items: center;
            justify-content: center;
            background-image: repeating-linear-gradient(45deg, #444 0px, #444 10px, #383838 10px, #383838 20px);
            position: relative;
            border-bottom: 3px solid var(--rust);
            overflow: hidden;
        }
        .card-img span {
            font-size: 4rem;
            filter: drop-shadow(5px 5px 2px rgba(0,0,0,0.7));
            transition: 0.3s;
        }
        .card:hover .card-img span {
            transform: scale(1.2) rotate(10deg);
        }
        .card-content {
            padding: 20px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }
        .card h3 {
            font-size: 1.4rem;
            color: #fff;
            margin-bottom: 10px;
            text-align: center;
        }
        .card .specs {
            list-style: none;
            margin: 15px 0;
            font-size: 0.9rem;
            color: #b8a68b;
        }
        .card .specs li {
            border-bottom: 1px dashed #4a3324;
            padding: 5px 0;
            display: flex;
            justify-content: space-between;
        }
        .price {
            font-size: 1.6rem;
            color: var(--gold);
            text-align: center;
            margin: 15px 0;
            font-weight: bold;
        }
        .card .btn {
            margin-top: auto;
            text-align: center;
        }

        /* Блок преимуществ */
        .features {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            max-width: 1000px;
            margin: 30px auto;
            text-align: center;
        }
        .feature-item {
            width: 200px;
            margin: 15px;
            padding: 20px;
            background: rgba(33, 21, 16, 0.8);
            border: 1px solid #4a3324;
            transition: 0.3s;
        }
        .feature-item:hover {
            border-color: var(--gold);
            transform: translateY(-5px);
        }
        .feature-item .icon {
            font-size: 3rem;
            margin-bottom: 15px;
        }
14:42
.feature-item h4 {
            color: var(--gold);
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        /* Форма связи */
        .contact-form {
            max-width: 600px;
            margin: 30px auto;
            padding: 30px;
            background: #211510;
            border: 2px solid var(--gold);
            box-shadow: 10px 10px 0px rgba(0,0,0,0.5);
        }
        .contact-form input, .contact-form textarea, .contact-form select {
            width: 100%;
            padding: 12px;
            margin-bottom: 15px;
            background: #1a1210;
            border: 1px solid #4a3324;
            color: #fff;
            font-family: 'Rubik', sans-serif;
        }
        .contact-form input:focus, .contact-form textarea:focus, .contact-form select:focus {
            border-color: var(--gold);
            outline: none;
        }

        footer {
            background: #0f0a08;
            color: #666;
            text-align: center;
            padding: 30px;
            border-top: 3px solid var(--gold);
            margin-top: 50px;
            font-size: 0.8rem;
            letter-spacing: 2px;
        }

        /* Анимации */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Адаптивность */
        @media (max-width: 768px) {
            .header-inner {
                flex-direction: column;
                text-align: center;
            }
            nav a {
                margin: 0 10px;
                font-size: 0.8rem;
            }
            .hero h2 {
                font-size: 2.5rem;
            }
        }
    </style>
</head>
<body>

    <!-- ШАПКА -->
    <header>
        <div class="header-inner">
            <div class="logo">
                <h1>ВЕЗЕТ КГ</h1>
                <p>Кованые прицепы · Испокон веков</p>
            </div>
            <nav>
                <a href="#catalog">Прицепы</a>
                <a href="#features">Качество</a>
                <a href="#contact">Контакты</a>
            </nav>
        </div>
    </header>

    <!-- ГЛАВНЫЙ ЭКРАН -->
    <section class="hero">
        <h2>Тяжелая <span>Работа</span><br>Для Железного Коня</h2>
        <div class="divider">⚒ ⚔ ⚒</div>
        <p>Изготавливаем прицепы для легковых автомобилей и квадроциклов. Металл толще, сварка крепче, дух — древнее.</p>
        <a href="#catalog" class="btn">Смотреть товары</a>
    </section>

    <!-- КАТАЛОГ -->
    <section id="catalog">
        <div class="section-title">⚙ Наша Кузница ⚙</div>
        <div class="catalog-grid">
            
            <!-- Товар 1 -->
            <div class="card">
                <div class="card-img"><span>🔩 </span></div>
                <div class="card-content">
                    <h3>Прицеп "Богатырь"</h3>
                    <ul class="specs">
                        <li>Грузоподъемность <span>500 кг</span></li>
                        <li>Кузов <span>Оцинковка</span></li>
                        <li>Подвеска <span>Рессорная</span></li>
                    </ul>
                    <div class="price">46 900 ₽</div>
                    <a href="#contact" class="btn">Заказать</a>
                </div>
            </div>

            <!-- Товар 2 -->
            <div class="card">
                <div class="card-img"><span>⚙</span></div>
                <div class="card-content">
                    <h3>Прицеп "Витязь"</h3>
                    <ul class="specs">
                        <li>Грузоподъемность <span>750 кг</span></li>
                        <li>Тент <span>В комплекте</span></li>
                        <li>Дышло <span>Усиленное</span></li>
                    </ul>
                    <div class="price">59 500 ₽</div>
                    <a href="#contact" class="btn">Заказать</a>
                </div>
            </div>

            <!-- Товар 3 -->
14:42
<div class="card">
                <div class="card-img"><span>🐎 </span></div>
                <div class="card-content">
                    <h3>Платформа "Квадро"</h3>
                    <ul class="specs">
                        <li>Размер <span>250x140 см</span></li>
                        <li>Трапы <span>Складные</span></li>
                        <li>Лебедка <span>Ручная</span></li>
                    </ul>
                    <div class="price">38 700 ₽</div>
                    <a href="#contact" class="btn">Заказать</a>
                </div>
            </div>
            
        </div>
    </section>

    <!-- ПРЕИМУЩЕСТВА -->
    <section id="features">
        <div class="section-title">✦ Почему Выбирают Нас ✦</div>
        <div class="features">
            <div class="feature-item">
                <div class="icon">🔥 </div>
                <h4>Ковка</h4>
                <p>Настоящий металл, а не фольга.</p>
            </div>
            <div class="feature-item">
                <div class="icon">🛡</div>
                <h4>Защита</h4>
                <p>Антикоррозийная обработка.</p>
            </div>
            <div class="feature-item">
                <div class="icon">📜 </div>
                <h4>Гарантия</h4>
                <p>Слово купца крепче договора.</p>
            </div>
        </div>
    </section>

    <!-- КОНТАКТЫ / ФОРМА -->
    <section id="contact">
        <div class="section-title">📯  Отправить Гонца 📯 </div>
        <div class="contact-form">
            <input type="text" placeholder="Имя твое, добрый человек *" required>
            <input type="tel" placeholder="Телефон для весточки *" required>
            <select>
                <option>Выбери товар</option>
                <option>Прицеп "Богатырь"</option>
                <option>Прицеп "Витязь"</option>
                <option>Платформа "Квадро"</option>
            </select>
            <textarea rows="3" placeholder="Комментарий (необязательно)"></textarea>
            <a href="#" class="btn" style="width:100%; text-align:center;" onclick="alert('Спасибо! Твой гонец уже скачет к нам. Мы свяжемся с тобой в ближайшее время.'); return false;">Отправить заявку</a>
        </div>
        <p style="text-align:center; color:#8a7a64;">Или звони напрямую: <span style="color:var(--gold); font-size:1.5rem;">+7 (900) 000-00-00</span></p>
    </section>

    <!-- ПОДВАЛ -->
    <footer>
        <p>© 2024 «Везет КГ». Все права защищены.</p>
        <p>Сделано с душой и молотом. 🛠</p>
    </footer>

</body>
</html>
