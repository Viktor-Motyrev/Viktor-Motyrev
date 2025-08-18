<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Добро пожаловать - Viktor-Motyrev</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
        }
        
        .welcome-container {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            text-align: center;
            max-width: 600px;
            animation: fadeInUp 1s ease-out;
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .avatar {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background: linear-gradient(45deg, #FF6B6B, #4ECDC4);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 48px;
            margin: 0 auto 20px;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            background: linear-gradient(45deg, #FFD700, #FF6B6B);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .subtitle {
            font-size: 1.2rem;
            margin-bottom: 30px;
            opacity: 0.9;
        }
        
        .stats {
            display: flex;
            justify-content: space-around;
            margin: 30px 0;
            flex-wrap: wrap;
            gap: 20px;
        }
        
        .stat-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 15px 20px;
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            flex: 1;
            min-width: 120px;
        }
        
        .stat-number {
            font-size: 2rem;
            font-weight: bold;
            color: #FFD700;
        }
        
        .stat-label {
            font-size: 0.9rem;
            opacity: 0.8;
            margin-top: 5px;
        }
        
        .projects {
            margin-top: 30px;
        }
        
        .projects h3 {
            margin-bottom: 20px;
            font-size: 1.5rem;
        }
        
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }
        
        .project-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
        }
        
        .project-name {
            font-weight: bold;
            margin-bottom: 8px;
            color: #4ECDC4;
        }
        
        .project-tech {
            background: rgba(255, 215, 0, 0.2);
            color: #FFD700;
            padding: 4px 8px;
            border-radius: 12px;
            font-size: 0.8rem;
            display: inline-block;
            margin-top: 8px;
        }
        
        .github-link {
            display: inline-block;
            margin-top: 30px;
            padding: 12px 24px;
            background: linear-gradient(45deg, #333, #666);
            color: white;
            text-decoration: none;
            border-radius: 25px;
            transition: transform 0.3s ease;
            font-weight: bold;
        }
        
        .github-link:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .emoji {
            font-size: 1.5rem;
            margin: 0 5px;
        }
    </style>
</head>
<body>
    <div class="welcome-container">
        <div class="avatar">👋</div>
        
        <h1>Привет, я Viktor!</h1>
        <p class="subtitle">Разработчик веб-приложений <span class="emoji">💻</span></p>
        
        <div class="stats">
            <div class="stat-item">
                <div class="stat-number">9</div>
                <div class="stat-label">Репозиториев</div>
            </div>
            <div class="stat-item">
                <div class="stat-number">1</div>
                <div class="stat-label">Подписчик</div>
            </div>
            <div class="stat-item">
                <div class="stat-number">6</div>
                <div class="stat-label">Основных проектов</div>
            </div>
        </div>
        
        <div class="projects">
            <h3>🚀 Мои проекты</h3>
            <div class="project-grid">
                <div class="project-card">
                    <div class="project-name">Веб Ларёк</div>
                    <div>Современный фронтенд для интернет-магазина</div>
                    <span class="project-tech">TypeScript</span>
                </div>
                
                <div class="project-card">
                    <div class="project-name">Mesto</div>
                    <div>Социальная сеть для фотографий</div>
                    <span class="project-tech">JavaScript</span>
                </div>
                
                <div class="project-card">
                    <div class="project-name">Оно тебе надо</div>
                    <div>Креативный веб-проект</div>
                    <span class="project-tech">HTML</span>
                </div>
                
                <div class="project-card">
                    <div class="project-name">Посмотри в окно</div>
                    <div>Интерактивное веб-приложение</div>
                    <span class="project-tech">JavaScript</span>
                </div>
                
                <div class="project-card">
                    <div class="project-name">Сложно сосредоточиться</div>
                    <div>Стильный веб-сайт</div>
                    <span class="project-tech">HTML</span>
                </div>
                
                <div class="project-card">
                    <div class="project-name">Закрывающий тег</div>
                    <div>Образовательный проект</div>
                    <span class="project-tech">HTML</span>
                </div>
            </div>
        </div>
        
        <a href="https://github.com/Viktor-Motyrev" class="github-link" target="_blank">
            🐙 Посетить мой GitHub
        </a>
        
        <p style="margin-top: 30px; opacity: 0.7; font-size: 0.9rem;">
            <span class="emoji">⚡</span> Увлечен современными технологиями и созданием качественных веб-приложений
        </p>
    </div>
</body>
</html>
