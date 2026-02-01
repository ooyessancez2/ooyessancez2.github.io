# ooyessancez2.github.io

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Parental Control Pro - Быстрая установка</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            color: white;
            padding: 20px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(0, 0, 0, 0.8);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .header {
            text-align: center;
            margin-bottom: 40px;
        }
        
        .header h1 {
            font-size: 3em;
            margin-bottom: 10px;
            background: linear-gradient(135deg, #00b4db, #0083b0);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .header p {
            font-size: 1.2em;
            opacity: 0.8;
        }
        
        .badge {
            display: inline-block;
            background: linear-gradient(135deg, #00b4db, #0083b0);
            color: white;
            padding: 8px 20px;
            border-radius: 50px;
            font-size: 0.9em;
            font-weight: bold;
            margin: 10px 5px;
        }
        
        .tabs {
            display: flex;
            gap: 10px;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }
        
        .tab-btn {
            background: rgba(255, 255, 255, 0.1);
            border: none;
            color: white;
            padding: 15px 30px;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-size: 1.1em;
        }
        
        .tab-btn.active {
            background: linear-gradient(135deg, #00b4db, #0083b0);
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(0, 180, 219, 0.3);
        }
        
        .tab-btn:hover:not(.active) {
            background: rgba(255, 255, 255, 0.2);
        }
        
        .tab-content {
            display: none;
            animation: fadeIn 0.5s ease;
        }
        
        .tab-content.active {
            display: block;
        }
        
        .install-step {
            background: rgba(255, 255, 255, 0.05);
            padding: 25px;
            border-radius: 15px;
            margin-bottom: 20px;
            border-left: 4px solid #00b4db;
        }
        
        .step-number {
            display: inline-block;
            background: #00b4db;
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            text-align: center;
            line-height: 40px;
            font-weight: bold;
            font-size: 1.2em;
            margin-right: 15px;
        }
        
        .code-block {
            background: rgba(0, 0, 0, 0.5);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            padding: 20px;
            margin: 20px 0;
            overflow-x: auto;
            font-family: 'Consolas', monospace;
        }
        
        .code-block code {
            color: #00ff9d;
            font-size: 0.95em;
            line-height: 1.5;
        }
        
        .btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 15px 30px;
            font-size: 1.1em;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: bold;
            text-decoration: none;
            margin: 10px 5px;
        }
        
        .btn-primary {
            background: linear-gradient(135deg, #00b4db, #0083b0);
            color: white;
        }
        
        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0, 180, 219, 0.3);
        }
        
        .btn-secondary {
            background: rgba(255, 255, 255, 0.1);
            color: white;
            border: 2px solid rgba(255, 255, 255, 0.3);
        }
        
        .btn-secondary:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateY(-3px);
        }
        
        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .feature-card {
            background: rgba(255, 255, 255, 0.05);
            padding: 25px;
            border-radius: 15px;
            text-align: center;
            transition: transform 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            background: rgba(255, 255, 255, 0.1);
        }
        
        .feature-icon {
            font-size: 3em;
            margin-bottom: 15px;
            color: #00b4db;
        }
        
        .screenshots {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 30px 0;
        }
        
        .screenshot {
            border-radius: 10px;
            overflow: hidden;
            border: 2px solid rgba(255, 255, 255, 0.3);
            transition: transform 0.3s ease;
        }
        
        .screenshot:hover {
            transform: scale(1.05);
        }
        
        .screenshot img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            display: block;
        }
        
        .screenshot-caption {
            padding: 15px;
            background: rgba(0, 0, 0, 0.5);
            text-align: center;
        }
        
        .info-box {
            background: rgba(0, 180, 219, 0.1);
            border: 1px solid rgba(0, 180, 219, 0.3);
            border-radius: 10px;
            padding: 20px;
            margin: 20px 0;
        }
        
        .warning-box {
            background: rgba(255, 193, 7, 0.1);
            border: 1px solid rgba(255, 193, 7, 0.3);
            border-radius: 10px;
            padding: 20px;
            margin: 20px 0;
        }
        
        .faq-item {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 15px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        
        .faq-item:hover {
            background: rgba(255, 255, 255, 0.1);
        }
        
        .faq-question {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-weight: bold;
            font-size: 1.1em;
        }
        
        .faq-answer {
            margin-top: 15px;
            display: none;
            color: rgba(255, 255, 255, 0.8);
        }
        
        .faq-item.active .faq-answer {
            display: block;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @media (max-width: 768px) {
            .container { padding: 20px; }
            .header h1 { font-size: 2em; }
            .tabs { flex-direction: column; }
            .tab-btn { width: 100%; }
            .btn { width: 100%; margin: 5px 0; }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Parental Control Pro v2.0</h1>
            <p>Профессиональная система родительского контроля</p>
            <div style="margin-top: 20px;">
                <span class="badge"><i class="fas fa-shield-alt"></i> Безопасность</span>
                <span class="badge"><i class="fas fa-bolt"></i> Быстрая установка</span>
                <span class="badge"><i class="fas fa-laptop"></i> Управление устройствами</span>
                <span class="badge"><i class="fas fa-clock"></i> Контроль времени</span>
            </div>
        </div>
        
        <div class="tabs">
            <button class="tab-btn active" onclick="showTab('quick')">
                <i class="fas fa-bolt"></i> Быстрая установка
            </button>
            <button class="tab-btn" onclick="showTab('server')">
                <i class="fas fa-server"></i> Установка сервера
            </button>
            <button class="tab-btn" onclick="showTab('client')">
                <i class="fas fa-laptop"></i> Установка клиента
            </button>
            <button class="tab-btn" onclick="showTab('features')">
                <i class="fas fa-star"></i> Возможности
            </button>
            <button class="tab-btn" onclick="showTab('faq')">
                <i class="fas fa-question-circle"></i> FAQ
            </button>
        </div>
        
        <!-- Быстрая установка -->
        <div id="quickTab" class="tab-content active">
            <h2><i class="fas fa-bolt"></i> 5-минутная установка</h2>
            <p>Следуйте этим простым шагам, чтобы начать работу:</p>
            
            <div class="install-step">
                <div class="step-number">1</div>
                <h3>Установите сервер на главный компьютер</h3>
                <p>Скачайте и запустите установщик сервера на компьютере, который будет управлять системой:</p>
                <div class="code-block">
                    <code>// Скопируйте этот код в файл server_install.bat</code><br>
                    <textarea id="serverCode" readonly style="width: 100%; height: 300px; background: transparent; border: none; color: #00ff9d; font-family: monospace; resize: none;"></textarea>
                </div>
                <button class="btn btn-primary" onclick="copyServerCode()">
                    <i class="far fa-copy"></i> Скопировать код установщика сервера
                </button>
            </div>
            
            <div class="install-step">
                <div class="step-number">2</div>
                <h3>Установите клиенты на другие компьютеры</h3>
                <p>Запустите установщик клиента на всех компьютерах, которые нужно контролировать:</p>
                <div class="code-block">
                    <code>// Скопируйте этот код в файл client_install.bat</code><br>
                    <textarea id="clientCode" readonly style="width: 100%; height: 300px; background: transparent; border: none; color: #00ff9d; font-family: monospace; resize: none;"></textarea>
                </div>
                <button class="btn btn-primary" onclick="copyClientCode()">
                    <i class="far fa-copy"></i> Скопировать код установщика клиента
                </button>
            </div>
            
            <div class="install-step">
                <div class="step-number">3</div>
                <h3>Откройте панель управления</h3>
                <p>После установки откройте браузер и перейдите по адресу:</p>
                <div class="code-block">
                    <code>http://localhost:8080</code>
                </div>
                <p>Используйте для входа:</p>
                <ul style="margin: 15px 0 15px 30px; color: rgba(255, 255, 255, 0.8);">
                    <li>Логин: <strong>admin</strong></li>
                    <li>Пароль: <strong>admin123</strong></li>
                </ul>
                <button class="btn btn-secondary" onclick="showTab('server')">
                    <i class="fas fa-server"></i> Подробная установка сервера
                </button>
                <button class="btn btn-secondary" onclick="showTab('client')">
                    <i class="fas fa-laptop"></i> Подробная установка клиента
                </button>
            </div>
            
            <div class="info-box">
                <h4><i class="fas fa-info-circle"></i> Важная информация</h4>
                <p>Установщики автоматически запрашивают права администратора и устанавливают все необходимые компоненты. После установки система запускается автоматически.</p>
            </div>
        </div>
        
        <!-- Установка сервера -->
        <div id="serverTab" class="tab-content">
            <h2><i class="fas fa-server"></i> Подробная установка сервера</h2>
            <p>Сервер устанавливается на компьютер, который будет управлять всей системой.</p>
            
            <div class="install-step">
                <h3><i class="fas fa-check-circle"></i> Требования</h3>
                <ul style="margin: 15px 0 15px 30px; color: rgba(255, 255, 255, 0.8);">
                    <li>Windows 10/11</li>
                    <li>Python 3.11+ (устанавливается автоматически)</li>
                    <li>Минимум 2GB оперативной памяти</li>
                    <li>Свободное место на диске: 100MB</li>
                </ul>
            </div>
            
            <div class="install-step">
                <h3><i class="fas fa-download"></i> Способ 1: Скачать готовый установщик</h3>
                <p>Скачайте готовый установщик сервера:</p>
                <button class="btn btn-primary" onclick="downloadServerInstaller()">
                    <i class="fas fa-download"></i> Скачать server_install.bat
                </button>
            </div>
            
            <div class="install-step">
                <h3><i class="fas fa-code"></i> Способ 2: Создать установщик вручную</h3>
                <p>Создайте файл <strong>server_install.bat</strong> и вставьте в него код:</p>
                <div class="code-block">
                    <textarea id="fullServerCode" readonly style="width: 100%; height: 400px; background: transparent; border: none; color: #00ff9d; font-family: monospace; resize: none;"></textarea>
                </div>
                <button class="btn btn-primary" onclick="copyFullServerCode()">
                    <i class="far fa-copy"></i> Скопировать полный код сервера
                </button>
            </div>
            
            <div class="install-step">
                <h3><i class="fas fa-play"></i> Запуск и настройка</h3>
                <p>После установки:</p>
                <ol style="margin: 15px 0 15px 30px; color: rgba(255, 255, 255, 0.8);">
                    <li>Запустите <strong>server.bat</strong> из папки <strong>C:\ParentalControlPro</strong></li>
                    <li>Откройте браузер и перейдите на <strong>http://localhost:8080</strong></li>
                    <li>Войдите с логином <strong>admin</strong> и паролем <strong>admin123</strong></li>
                    <li>Измените пароль в настройках безопасности</li>
                </ol>
            </div>
            
            <div class="warning-box">
                <h4><i class="fas fa-exclamation-triangle"></i> Внимание!</h4>
                <p>При первом запуске установщик запросит права администратора. Это необходимо для установки Python и создания службы Windows.</p>
            </div>
        </div>
        
        <!-- Установка клиента -->
        <div id="clientTab" class="tab-content">
            <h2><i class="fas fa-laptop"></i> Установка клиента на устройства</h2>
            <p>Клиент устанавливается на все компьютеры, которые нужно контролировать.</p>
            
            <div class="install-step">
                <h3><i class="fas fa-network-wired"></i> Перед установкой</h3>
                <p>Узнайте IP адрес сервера. Запустите на сервере и посмотрите в консоли или используйте команду:</p>
                <div class="code-block">
                    <code>ipconfig</code>
                </div>
                <p>Найдите строку "IPv4 Address". Обычно это что-то вроде <strong>192.168.1.100</strong></p>
            </div>
            
            <div class="install-step">
                <h3><i class="fas fa-download"></i> Способ 1: Скачать готовый установщик</h3>
                <p>Скачайте установщик клиента:</p>
                <button class="btn btn-primary" onclick="downloadClientInstaller()">
                    <i class="fas fa-download"></i> Скачать client_install.bat
                </button>
            </div>
            
            <div class="install-step">
                <h3><i class="fas fa-code"></i> Способ 2: Создать установщик вручную</h3>
                <p>Создайте файл <strong>client_install.bat</strong> и вставьте в него код:</p>
                <div class="code-block">
                    <textarea id="fullClientCode" readonly style="width: 100%; height: 400px; background: transparent; border: none; color: #00ff9d; font-family: monospace; resize: none;"></textarea>
                </div>
                <button class="btn btn-primary" onclick="copyFullClientCode()">
                    <i class="far fa-copy"></i> Скопировать полный код клиента
                </button>
            </div>
            
            <div class="install-step">
                <h3><i class="fas fa-cogs"></i> Настройка подключения</h3>
                <p>При запуске клиента вас попросят ввести IP адрес сервера. Введите тот адрес, который вы нашли ранее.</p>
                <p>Клиент автоматически:</p>
                <ul style="margin: 15px 0 15px 30px; color: rgba(255, 255, 255, 0.8);">
                    <li>Зарегистрируется на сервере</li>
                    <li>Добавится в автозагрузку</li>
                    <li>Начнет отправлять статистику</li>
                    <li>Будет выполнять команды с сервера</li>
                </ul>
            </div>
            
            <div class="info-box">
                <h4><i class="fas fa-lightbulb"></i> Совет</h4>
                <p>Для удобства можно создать ярлык client_install.bat на флешку и запускать его на всех компьютерах, которые нужно подключить к системе.</p>
            </div>
        </div>
        
        <!-- Возможности -->
        <div id="featuresTab" class="tab-content">
            <h2><i class="fas fa-star"></i> Возможности системы</h2>
            
            <div class="feature-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-laptop-house"></i>
                    </div>
                    <h3>Управление устройствами</h3>
                    <p>Контролируйте все компьютеры в сети через единую панель управления</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>Автоадминистратор</h3>
                    <p>Автоматическое получение прав администратора без подтверждения</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-filter"></i>
                    </div>
                    <h3>Фильтрация контента</h3>
                    <p>Гибкая настройка белых списков сайтов и приложений</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-clock"></i>
                    </div>
                    <h3>Расписание доступа</h3>
                    <p>Ограничение времени использования по дням недели</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-ban"></i>
                    </div>
                    <h3>Блокировка</h3>
                    <p>Удаленная блокировка компьютеров, выключение, перезагрузка</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3>Статистика</h3>
                    <p>Детальная статистика использования и активности</p>
                </div>
            </div>
            
            <h3 style="margin-top: 40px;"><i class="fas fa-desktop"></i> Скриншоты интерфейса</h3>
            <div class="screenshots">
                <div class="screenshot">
                    <img src="https://via.placeholder.com/400x200/00b4db/ffffff?text=Панель+управления" alt="Панель управления">
                    <div class="screenshot-caption">Панель управления устройствами</div>
                </div>
                <div class="screenshot">
                    <img src="https://via.placeholder.com/400x200/0083b0/ffffff?text=Настройки+белого+списка" alt="Настройки белого списка">
                    <div class="screenshot-caption">Настройки белого списка</div>
                </div>
                <div class="screenshot">
                    <img src="https://via.placeholder.com/400x200/764ba2/ffffff?text=Статистика+использования" alt="Статистика использования">
                    <div class="screenshot-caption">Статистика использования</div>
                </div>
            </div>
        </div>
        
        <!-- FAQ -->
        <div id="faqTab" class="tab-content">
            <h2><i class="fas fa-question-circle"></i> Часто задаваемые вопросы</h2>
            
            <div class="faq-item" onclick="toggleFaq(this)">
                <div class="faq-question">
                    <span>Как изменить пароль по умолчанию?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    После входа в панель управления перейдите в раздел "Настройки" → "Безопасность" и измените пароль администратора.
                </div>
            </div>
            
            <div class="faq-item" onclick="toggleFaq(this)">
                <div class="faq-question">
                    <span>Как подключить больше компьютеров?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    Просто запустите client_install.bat на каждом компьютере, который нужно подключить. Введите IP адрес сервера при установке.
                </div>
            </div>
            
            <div class="faq-item" onclick="toggleFaq(this)">
                <div class="faq-question">
                    <span>Можно ли управлять системой с телефона?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    Да! Откройте браузер на телефоне и перейдите по адресу http://IP_сервера:8080. Интерфейс адаптирован для мобильных устройств.
                </div>
            </div>
            
            <div class="faq-item" onclick="toggleFaq(this)">
                <div class="faq-question">
                    <span>Как добавить сайт в белый список?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    В панели управления выберите устройство → "Белый список" → "Добавить сайт". Можно использовать маски типа *.youtube.com
                </div>
            </div>
            
            <div class="faq-item" onclick="toggleFaq(this)">
                <div class="faq-question">
                    <span>Система требует права администратора. Это безопасно?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    Да, это безопасно. Права администратора нужны для блокировки сайтов через файл hosts и управления приложениями. Код открыт для проверки.
                </div>
            </div>
            
            <div class="faq-item" onclick="toggleFaq(this)">
                <div class="faq-question">
                    <span>Как отключить клиент на компьютере?</span>
                    <i class="fas fa-chevron-down"></i>
                </div>
                <div class="faq-answer">
                    Удалите файл из автозагрузки: %APPDATA%\Microsoft\Windows\Start Menu\Programs\Startup\ParentalControlClient.vbs
                </div>
            </div>
            
            <div class="info-box" style="margin-top: 30px;">
                <h4><i class="fas fa-life-ring"></i> Нужна помощь?</h4>
                <p>Если у вас возникли проблемы с установкой или использованием системы:</p>
                <ol style="margin: 15px 0 15px 30px; color: rgba(255, 255, 255, 0.8);">
                    <li>Проверьте, что брандмауэр не блокирует порт 8080</li>
                    <li>Убедитесь, что все компьютеры в одной сети</li>
                    <li>Перезапустите сервер и клиенты</li>
                    <li>Проверьте логи в папках C:\ParentalControlPro\logs и C:\ParentalControlClient\logs</li>
                </ol>
            </div>
        </div>
        
        <div style="margin-top: 50px; padding-top: 30px; border-top: 1px solid rgba(255, 255, 255, 0.1); text-align: center;">
            <p>Parental Control Pro v2.0 | Система родительского контроля нового поколения</p>
            <p style="margin-top: 10px; font-size: 0.9em; color: rgba(255, 255, 255, 0.6);">
                Скачайте, установите и начинайте управлять устройствами уже через 5 минут!
            </p>
            <div style="margin-top: 20px;">
                <button class="btn btn-primary" onclick="showTab('quick')">
                    <i class="fas fa-bolt"></i> Начать установку
                </button>
            </div>
        </div>
    </div>
    
    <script>
        // Показываем выбранную вкладку
        function showTab(tabName) {
            // Скрываем все вкладки
            document.querySelectorAll('.tab-content').forEach(tab => {
                tab.classList.remove('active');
            });
            
            // Убираем активный класс со всех кнопок
            document.querySelectorAll('.tab-btn').forEach(btn => {
                btn.classList.remove('active');
            });
            
            // Показываем выбранную вкладку
            document.getElementById(tabName + 'Tab').classList.add('active');
            
            // Делаем активной кнопку вкладки
            event.currentTarget.classList.add('active');
        }
        
        // Переключение FAQ
        function toggleFaq(element) {
            element.classList.toggle('active');
        }
        
        // Коды установщиков (сокращенные для примера)
        const serverCode = `@echo off\nchcp 65001 >nul\ntitle Parental Control Pro - Установка сервера\n\n:: Автоматическое получение прав администратора\n:: Установка Python и зависимостей\n:: Создание веб-интерфейса\n:: Настройка службы Windows\n\necho Установка завершена!\npause`;
        const clientCode = `@echo off\nchcp 65001 >nul\ntitle Parental Control Pro - Установка клиента\n\n:: Автоматическое получение прав администратора\n:: Регистрация на сервере\n:: Добавление в автозагрузку\n\necho Установка завершена!\npause`;
        
        // Полные коды (в реальности здесь будут полные коды из первых двух файлов)
        const fullServerCode = `Полный код server_install.bat будет здесь`;
        const fullClientCode = `Полный код client_install.bat будет здесь`;
        
        // Заполняем текстовые области при загрузке
        document.addEventListener('DOMContentLoaded', function() {
            document.getElementById('serverCode').value = serverCode;
            document.getElementById('clientCode').value = clientCode;
            document.getElementById('fullServerCode').value = fullServerCode;
            document.getElementById('fullClientCode').value = fullClientCode;
        });
        
        // Функции копирования
        function copyServerCode() {
            copyToClipboard(serverCode);
            alert('Код установщика сервера скопирован в буфер обмена!');
        }
        
        function copyClientCode() {
            copyToClipboard(clientCode);
            alert('Код установщика клиента скопирован в буфер обмена!');
        }
        
        function copyFullServerCode() {
            copyToClipboard(fullServerCode);
            alert('Полный код сервера скопирован в буфер обмена!');
        }
        
        function copyFullClientCode() {
            copyToClipboard(fullClientCode);
            alert('Полный код клиента скопирован в буфер обмена!');
        }
        
        function copyToClipboard(text) {
            const textarea = document.createElement('textarea');
            textarea.value = text;
            document.body.appendChild(textarea);
            textarea.select();
            document.execCommand('copy');
            document.body.removeChild(textarea);
        }
        
        // Функции загрузки (в реальном сайте будут ссылки на файлы)
        function downloadServerInstaller() {
            const content = serverCode;
            const blob = new Blob([content], { type: 'text/plain' });
            const url = window.URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = 'server_install.bat';
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            window.URL.revokeObjectURL(url);
            alert('Файл server_install.bat скачан!');
        }
        
        function downloadClientInstaller() {
            const content = clientCode;
            const blob = new Blob([content], { type: 'text/plain' });
            const url = window.URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = 'client_install.bat';
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            window.URL.revokeObjectURL(url);
            alert('Файл client_install.bat скачан!');
        }
        
        // Автоматическое открытие FAQ при клике
        document.querySelectorAll('.faq-item').forEach(item => {
            item.addEventListener('click', function() {
                this.classList.toggle('active');
            });
        });
    </script>
</body>
</html>
