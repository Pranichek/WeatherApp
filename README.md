<h1>WEATHER APPLICATION</h1>

<p style='text-align:  justify;'> 
    <span style='margin-left: 40px;'>Цей</span> 
    проєкт розроблено з метою ознайомлення із роботою 
    <a href='https://developer.mozilla.org/en-US/docs/Glossary/API'>API</a>, 
    принципом отримання даних від віддаленого серверу, вмінням обробляти дані, структурувати та застосовувати у свому проєкті. А саме застосовувалось API такого веб-ресурсу як 
    <a href='https://openweathermap.org/'>OpenWeatherMap</a>.
    Проєкт допоможе розібратисяс у роботі файлів
    <a href='https://www.json.org/json-uk.html'>JSON</a>, 
    як правильно отримувати та зберігати дані у файлах з типом json. Та познайомить користувача з інтерфейсом застосунку розробленим за допомогою пакету 
    <a href='https://customtkinter.tomschimansky.com/'>Custotkinter</a>.
</p>

<img src='/static/icon/screen.png'>

<h2 id="structure">Зміст:</h2>
<ol>
    <li>
        <a href='#all-modules'>Модулі проєкту</a>.
    </li>
    <li>
        <a href='#download-project'>Розгортання проєкту</a>.
    </li>
    <li>
        <a href='#create-venv'>Створення віртуального оточення</a>.
        <ul>
            <li>
                <a href='#windows'>Для Windows</a>.
            </li>
            <li>
                <a href='#mac-os'>Для Mac OS</a>.
            </li>
        </ul>
    </li>
    <li>
        <a href='#download-modules'>Завантаження модулей до віртуального проєкту</a>.
        <ul>
            <li>
                <a href='#requriments'>Завантаження requriments.txt</a>.
            </li>
            <li>
                <a href='#pip-install'>Завантаження окремих модулів</a>.
            </li>
        </ul>
    </li>
    <li>
        <a href='#start-project'>Старт проєкту</a>.
    </li>
    <li>
        <a href='#base-mechanics'>Основні механіки проєкту</a>.
    </li>
    <li>
        <a href='#result'>Висновок</a>.
    </li>
</ol>

<hr>

<h3 id='download-project'>Розгортання проєкту</h3>

<ol>
    <li>Склонуйте репозиторій на свій комп'ютер за допомогою git:
        <pre><code>git clone https://github.com/Pranichek/WeatherApp.git</code></pre>
    </li>
    <li>Перейдіть у директорію проєкту:
        <pre><code>cd WeatherApp</code></pre>
    </li>
</ol>

<p>
    Тепер ви готові до подальших кроків з налаштування віртуального оточення та встановлення залежностей.
</p>

<a href='#structure' style='text-decoration: none; color: black; font-weight: 600;'>Повернутися до змісту ⬆️</a>
<hr>

<h3 id='all-modules'>Модулі проєкту</h3>

<h3>Модулі для завантаження</h3> 


<ul>
    <li><span style='font-weight: 600'>customtkinter</span> - модуль для створення десктоп-додатків з сучасним графічним інтерфейсом у Python.</li>
    <li><span style='font-weight: 600'>requests</span> — це бібліотека для виконання HTTP-запитів у зручному вигляді.</li>
    <li><span style='font-weight: 600'>pillow</span> — це модуль, який використовується для обробки зображень.</li>
</ul>


<h3>Стандартні модулі</h3>
<ul>
    <li><span style='font-weight: 600;'>os</span> - модуль, який використовується для побудови шляхів до файлів, роботи з директоріями.</li>
    <li><span style='font-weight: 600;'>json</span> - стандартний модуль Python для збереження та обміну структурованими даними у форматі JSON.</li>
</ul>

<a href='#structure' style='text-decoration: none; color: black; font-weight: 600;'>Повернутися до змісту ⬆️</a>
<hr>

<h3 id='download-project'>Розгортання проєкту</h3>

<h3 id='create-venv'>Створення віртуального оточення</h3>

<p>
    Для ізоляції залежностей проєкту рекомендується створити віртуальне оточення. Це дозволяє уникнути конфліктів між бібліотеками різних проєктів.
</p>

<h4 id='windows'>Для Windows:</h4>

<ol>
    <li>Відкрийте <b>Command Prompt</b> або <b>PowerShell</b>.</li>
    <li>Перейдіть у директорію проєкту:
        <pre><code>cd WeatherApp</code></pre>
    </li>
    <li>Створіть віртуальне оточення:
        <pre><code>python -m venv venv</code></pre>
    </li>
    <li>Активуйте віртуальне оточення:
        <pre><code>venv\Scripts\activate</code></pre>
    </li>
</ol>

<h4 id='mac-os'>Для Mac OS:</h4>

<ol>
    <li>Відкрийте <b>Terminal</b>.</li>
    <li>Перейдіть у директорію проєкту:
        <pre><code>cd WeatherApp</code></pre>
    </li>
    <li>Створіть віртуальне оточення:
        <pre><code>python3 -m venv venv</code></pre>
    </li>
    <li>Активуйте віртуальне оточення:
        <pre><code>source venv/bin/activate</code></pre>
    </li>
</ol>

<p>
    Після активації віртуального оточення ви побачите відповідний префікс у командному рядку. Тепер можна встановлювати необхідні бібліотеки, не впливаючи на глобальні налаштування Python.
</p>

<a href='#structure' style='text-decoration: none; color: black; font-weight: 600;'>Повернутися до змісту ⬆️</a>
<hr>
<h3 id='download-modules'>Завантаження модулів до віртуального оточення</h3>

<p>
    Після створення та активації віртуального оточення потрібно встановити необхідні модулі для роботи проєкту.
</p>

<h4 id='requriments'>Завантаження через requirements.txt</h4>

<ol>
    <li><b>Для Windows:</b>
        <ul>
            <li>Переконайтесь, що ви знаходитеся у директорії проєкту та активували віртуальне оточення.</li>
            <li>Виконайте команду:
                <pre><code>pip install -r requirements.txt</code></pre>
            </li>
        </ul>
    </li>
    <li><b>Для MacOS/Linux:</b>
        <ul>
            <li>Переконайтесь, що ви знаходитеся у директорії проєкту та активували віртуальне оточення.</li>
            <li>Виконайте команду:
                <pre><code>pip3 install -r requirements.txt</code></pre>
            </li>
        </ul>
    </li>
    <li><span id="pip-install" style="font-weight: 600">Приклад встановлення окремих модулів:</span>
        <ul>
            <li><span>Для Windows</span>:
                <pre><code>pip install customtkinter requests pillow</code></pre>
            </li>
            <li>Для MacOS/Linux:
                <pre><code>pip3 install customtkinter requests pillow</code></pre>
            </li>
        </ol>
    </li>
</ol>





<a href='#structure' style='text-decoration: none; color: black; font-weight: 600;'>Повернутися до змісту ⬆️</a>
<hr>

<h3 id='start-project'>Старт проєкту</h3>

<ol>
    <li>Переконайтесь, що всі необхідні модулі встановлені та віртуальне оточення активоване.</li>
    <li>Запустіть головний файл проєкту командою:
        <pre><code>python main.py</code></pre>
        <span>або для MacOS/Linux:</span>
        <pre><code>python3 main.py</code></pre>
    </li>
</ol>

<p>
    Після запуску відкриється графічний інтерфейс застосунку, де ви зможете переглядати актуальну погоду для обраного міста.
</p>

<a href='#structure' style='text-decoration: none; color: black; font-weight: 600;'>Повернутися до змісту ⬆️</a>
<hr>
<h3 id='base-mechanics'>Основні механіки проєкту</h3>

<ul>
    <li><b>Отримання даних:</b> Додаток надсилає запит до API <a href='https://openweathermap.org/'>OpenWeatherMap</a> для отримання актуальної інформації про погоду.</li>
    <li><b>Обробка відповіді:</b> Отримані дані у форматі JSON обробляються для подальшого відображення.</li>
    <li><b>Відображення інформації:</b> На екрані відображаються основні погодні параметри: температура, стан неба,  тощо.</li>
    <li><b>Оновлення даних:</b> Інформація про погоду та місто оновлюється автоматично при запуску застосунку.</li>
    <li><b>Графічний інтерфейс:</b> Всі елементи інтерфейсу створені за допомогою <b>customtkinter</b> для сучасного вигляду та зручності використання.</li>
    <li><b>Об'єктно-орієнтована структура:</b> Вся структура коду побудована на основі класів, що забезпечує зручність розширення, підтримки та повторного використання коду.</li>
</ul>
</ul>

<a href='#structure' style='text-decoration: none; color: black; font-weight: 600;'>Повернутися до змісту ⬆️</a>
<hr>

<h3 id='result'>Висновок</h3>

<p>
    Даний проєкт є чудовим прикладом використання API для отримання та обробки даних у реальному часі.Я ознайомився з принципами роботи з віддаленими серверами,так навчився працювати з форматом JSON, а також отримав досвід створення сучасного графічного інтерфейсу за допомогою <b>customtkinter</b>. Проєкт може стати основою для подальшого розвитку та додавання нових функцій, таких як розширена аналітика погоди, підтримка декількох мов або інтеграція з іншими сервісами.
</p>

<a href='#structure' style='text-decoration: none; color: black; font-weight: 600;'>Повернутися до змісту ⬆️</a>