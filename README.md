# Pancake Protectors Bot via computer vision (Windows)
## Локальне налаштування

### **Віртуальне середовище**

* Оновіть `venv` до останньої версії:
    ```
    pip install --upgrade virtualenv
    ```
* Створіть віртуальне середовище:
    ```
    python -m venv venv
    ```

* Активуйте віртуальне середовище
    * Windows
        ```
        .\venv\Scripts\activate
        ```

### **Встановлення залежностей**

* Оновіть `pip` до останьої версії:
    ```
    python -m pip install --upgrade pip
    ```
* Встановіть пакети зі списку що знаходиться у файлі:
    ```
    pip install -r .\requirements.txt
    ```
* **Встановіть сервіс для розпізнавання тексту**
  - Завантажити можна за посиланням https://github.com/UB-Mannheim/tesseract/wiki
  - Встановити у директорію `PP_Bot/services/Tesseract-OCR/`

## Використання
### **Запуск програми**
* Перед запуском програми необхідно перейти в кореневу директорію програми та редагувати / видалити файл `WHITELIST.txt` в якому вказуються назви руди, для яких функція `FARM MINE` припинить виконання (кожна назва з нового рядку)
    ```txt
    Ruby
    Gold
    Platinum
    Saltpeter
    ...
    ```

* Запустіть програму:
    ```
    python .\main.py
    ```
### **Інтерфейс**
- Виконання програми можна зупинити в будь-який момент натиснувши клавішу `ESC`

- Оберіть зі списку функцію, яка вам необхідна, або ж активуйте всі функції за допомогою чекбоксу `ВИБРАТИ ВСІ`

- Для функції `JOIN TO ARENA` є можливість обрати кількість циклів для виконання (за замовчуванням 1).

- Для функції `FARM MINE` є можливість обрати кількість циклів для виконання, якщо всі квести завершено (за замовчуванням 0 - функція виконуватиметься до тих пір, поки не закінчиться енергія, або поки не завершаться квести).

- авторизуйтесь на https://protectors.pancakeswap.finance та розташуйте вікно на передній план не менше ніж на 1/2 екрану.

- Натисніть `Почати` та після закінчення відліку бот автоматично знайде вікно застосунку і виконає попередньо обрані вами дії.

### **Рекомендації**
- під час використання рекомендується не ворушити курсором, та не відкривати інші вікна, оскільки курсор та картинка на екрані необхідні для коректної роботи бота.
- вікно редактора та консоль можна для зручності розташувати з іншого боку екрану, або ж на задньому фоні.
