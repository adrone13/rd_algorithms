### Завдання №3
Макс оцінка: 15 балів

Розробляючи систему для підказок при введенні адреси, нам необхідно реалізувати базовий двигун для пошуку.

Ми визначили два базові варіанти, які нам потрібно обробляти при пошуку:
* пошук за точною адресою: якщо у нас є точно те, що ввів користувач, наприклад "airport kbp"
* пошук за префікcом: якщо користувач вводить адресу і чекає на підказку, наприклад "airpo"

Для простоти реалізації ми будемо працювати з адресами у вигляді звичайного рядка, жодних складних об'єктів.

Також для простоти в контексті даного завдання вимоги до структури будуть дещо спрощені, а саме:
* можна розраховувати, що вся структура поміститься в памʼять, і нам НЕ потрібно видаляти з неї елементи
* insert(str): додає рядок до структури
* search(str): повертає TRUE якщо точно такий самий рядок є в структурі, інакше FALSE
* startsWith(prefix): повертає TRUE якщо є адреса з таким префіксом, інакше FALSE
* кількість пошуків перевищує кількість вставок, але операції можуть виконуватись у будь-якому порядку

Потрібно реалізувати структуру для такого пошукового двигуна. Шаблон лежить в tasks/T03/Trie. Вказуйте складність для методів в коді.

Також опишіть у парі слів вашу ідею, наприклад: "використовую структуру <$> для <$>, це дає швидкий доступ. Додатково зберігаю спеціальні прапори для того, щоб рахувати <$>"

Тести потрібні, але підготованих тестів у шаблоні нема. Вам потрібно самим написати їх і переконатися, що ви врахували всі варіанти.

Як написати тести – на ваш розсуд. Звичайні принти в консоль у вигляді "true" або "false", або assert, або, що вам подобається під кожен тест кейс теж підходять. 
Головне показати як ви тестуєте та які кейси продумуєте.

Обмеження:
* 1 <= str.length, prefix.length <= 2000
* всі адреси складаються лише з літер [a-z]

Оптимальність операцій на ваш розсуд, але, звичайно, треба добитися найкращого перформансу.