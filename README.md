Проект Referral System API
Проект Referral System API предоставляет возможность регистрации пользователей с использованием реферальных кодов, получения информации о рефералах и другие функции.

Инструкции по запуску
Установите необходимые зависимости:

!pip install Flask requests cachetools

Укажите свой API ключ Clearbit в коде:

api_key = 'YOUR_CLEARBIT_API_KEY'

Запустите приложение:

python your_file_name.py

Инструкции по тестированию
Для регистрации нового пользователя отправьте POST запрос на /register с JSON данными, например:

{
"email": "example@example.com",
"referral_code": "123456"
}

Для получения информации о рефералах по id реферера отправьте GET запрос на /referrals/, например:

GET /referrals/123456

Для получения реферального кода по email адресу реферера отправьте GET запрос на /referral-code/, например:

GET /referral-code/example@example.com

Проверьте ответы на запросы и убедитесь, что функциональность работает корректно.
Документация API
Документация API доступна по адресу http://localhost:5000/swagger или http://localhost:5000/redoc после запуска приложения.
