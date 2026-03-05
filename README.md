<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart AVR System — Розумне керування живленням</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        body { background-color: #0f172a; color: #f8fafc; scroll-behavior: smooth; }
        .gradient-text {
            background: linear-gradient(90deg, #38bdf8, #818cf8);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        [data-lang] { display: none; }
        body[data-current-lang="uk"] [data-lang="uk"] { display: block; }
        body[data-current-lang="en"] [data-lang="en"] { display: block; }
        body[data-current-lang="ru"] [data-lang="ru"] { display: block; }
        
        span[data-lang] { display: none !important; }
        body[data-current-lang="uk"] span[data-lang="uk"] { display: inline !important; }
        body[data-current-lang="en"] span[data-lang="en"] { display: inline !important; }
        body[data-current-lang="ru"] span[data-lang="ru"] { display: inline !important; }
    </style>
</head>
<body data-current-lang="uk">

    <nav class="p-6 flex justify-between items-center max-w-7xl mx-auto border-b border-slate-800">
        <div class="text-2xl font-bold tracking-tighter uppercase">Smart <span class="text-blue-500">AVR</span></div>
        <div class="flex items-center space-x-4">
            <select onchange="changeLang(this.value)" class="bg-slate-800 text-sm border border-slate-700 rounded px-2 py-1 outline-none cursor-pointer hover:bg-slate-700 transition">
                <option value="uk">UA</option>
                <option value="en">EN</option>
                <option value="ru">RU</option>
            </select>
            <a href="#contact" class="bg-blue-600 px-5 py-2 rounded-full text-sm font-bold hover:bg-blue-700 transition">
                <span data-lang="uk">Консультація</span>
                <span data-lang="en">Get in touch</span>
                <span data-lang="ru">Консультация</span>
            </a>
        </div>
    </nav>

    <section class="py-24 px-6 text-center">
        <div class="inline-block px-4 py-1 border border-blue-500/30 rounded-full text-blue-400 text-sm font-medium mb-6 bg-blue-500/5 uppercase tracking-widest">
            Industrial Control Systems
        </div>
        <h1 class="text-5xl md:text-7xl font-extrabold mb-8 leading-tight">
            <span data-lang="uk">Керуйте енергією</span>
            <span data-lang="en">Manage your energy</span>
            <span data-lang="ru">Управляйте энергией</span>
            <br>
            <span class="gradient-text">
                <span data-lang="uk">через Telegram</span>
                <span data-lang="en">via Telegram</span>
                <span data-lang="ru">через Telegram</span>
            </span>
        </h1>
        <p class="text-gray-400 text-xl max-w-3xl mx-auto mb-12">
            <span data-lang="uk">Професійна автоматика для вашого будинку. Повний моніторинг мережі, запуск генератора та перемикання режимів в один клік у вашому смартфоні.</span>
            <span data-lang="en">Professional automation for your home. Full network monitoring, generator start, and mode switching with one click on your smartphone.</span>
            <span data-lang="ru">Профессиональная автоматика для вашего дома. Полный мониторинг сети, запуск генератора и переключение режимов в один клик в вашем смартфоне.</span>
        </p>
    </section>

    <section class="py-16 bg-slate-900/40 border-y border-slate-800">
        <div class="max-w-6xl mx-auto px-6 flex flex-col md:flex-row items-center gap-16">
            <div class="md:w-1/2">
                <img src="image_1.png" alt="Telegram Interface" class="rounded-3xl shadow-2xl shadow-blue-500/10 border-4 border-slate-800 mx-auto max-w-[320px]">
            </div>
            <div class="md:w-1/2 text-left">
                <h2 class="text-4xl font-bold mb-6">
                    <span data-lang="uk">Ваш смартфон — <br>центр керування</span>
                    <span data-lang="en">Your smartphone is <br>the control center</span>
                    <span data-lang="ru">Ваш смартфон — <br>центр управления</span>
                </h2>
                <div class="space-y-6">
                    <div class="flex items-start gap-4">
                        <div class="p-3 bg-blue-600/20 rounded-lg"><i class="fa-solid fa-bolt text-blue-400"></i></div>
                        <div>
                            <h4 class="font-bold text-xl"><span data-lang="uk">Миттєві сповіщення</span><span data-lang="en">Instant Alerts</span><span data-lang="ru">Мгновенные уведомления</span></h4>
                            <p class="text-gray-400"><span data-lang="uk">Система повідомить вас у Telegram, коли зникне мережа або запуститься генератор.</span><span data-lang="en">The system will notify you in Telegram when the grid goes down or the generator starts.</span><span data-lang="ru">Система уведомит вас в Telegram, когда пропадет сеть или запустится генератор.</span></p>
                        </div>
                    </div>
                    <div class="flex items-start gap-4">
                        <div class="p-3 bg-blue-600/20 rounded-lg"><i class="fa-solid fa-sliders text-blue-400"></i></div>
                        <div>
                            <h4 class="font-bold text-xl"><span data-lang="uk">Вибір режимів</span><span data-lang="en">Mode Selection</span><span data-lang="ru">Выбор режимов</span></h4>
                            <p class="text-gray-400"><span data-lang="uk">Автоматичний, Ручний, Інвертор або Гібрид — керуйте логікою дистанційно.</span><span data-lang="en">Auto, Manual, Inverter, or Hybrid — manage the logic remotely.</span><span data-lang="ru">Автоматический, Ручной, Инвертор или Гибрид — управляйте логикой дистанционно.</span></p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="py-24 px-6 max-w-7xl mx-auto grid md:grid-cols-3 gap-12 text-center">
        <div>
            <div class="text-blue-500 text-3xl mb-4"><i class="fa-solid fa-server"></i></div>
            <h3 class="text-xl font-bold mb-2">Web-Interface</h3>
            <p class="text-gray-400 text-sm">
                <span data-lang="uk">Вбудований веб-сервер для детального налаштування параметрів через будь-який браузер.</span>
                <span data-lang="en">Built-in web server for detailed parameter settings via any browser.</span>
                <span data-lang="ru">Встроенный веб-сервер для детальной настройки параметров через любой браузер.</span>
            </p>
        </div>
        <div>
            <div class="text-blue-500 text-3xl mb-4"><i class="fa-solid fa-shield-check"></i></div>
            <h3 class="text-xl font-bold mb-2">Smart Safety</h3>
            <p class="text-gray-400 text-sm">
                <span data-lang="uk">Багаторівневий захист від зустрічної напруги та перевантажень на програмному рівні.</span>
                <span data-lang="en">Multi-level protection against counter-voltage and overloads at the software level.</span>
                <span data-lang="ru">Многоуровневая защита от встречного напряжения и перегрузок на программном уровне.</span>
            </p>
        </div>
        <div>
            <div class="text-blue-500 text-3xl mb-4"><i class="fa-solid fa-microchip"></i></div>
            <h3 class="text-xl font-bold mb-2">Pro Logic</h3>
            <p class="text-gray-400 text-sm">
                <span data-lang="uk">Інтелектуальні алгоритми прогріву та охолодження генератора.</span>
                <span data-lang="en">Intelligent algorithms for generator warm-up.</span>
                <span data-lang="ru">Интеллектуальные алгоритмы прогрева и охлаждения генератора.</span>
            </p>
        </div>
    </section>

    <footer id="contact" class="py-20 text-center border-t border-slate-800">
        <h2 class="text-3xl font-bold mb-10">
            <span data-lang="uk">Готові до автоматизації?</span>
            <span data-lang="en">Ready for automation?</span>
            <span data-lang="ru">Готовы к автоматизации?</span>
        </h2>
        <a href="https://t.me/opc_driver" class="bg-blue-600 px-10 py-4 rounded-full text-lg font-bold hover:bg-blue-700 transition">
            <i class="fa-brands fa-telegram mr-2"></i>
            <span data-lang="uk">Написати розробнику</span>
            <span data-lang="en">Contact Developer</span>
            <span data-lang="ru">Написать разработчику</span>
        </a>
    </footer>

    <script>
        function changeLang(lang) {
            document.body.setAttribute('data-current-lang', lang);
            localStorage.setItem('preferredLang', lang);
        }
        const savedLang = localStorage.getItem('preferredLang') || 'uk';
        document.body.setAttribute('data-current-lang', savedLang);
        document.querySelector('select').value = savedLang;
    </script>
</body>
</html>
