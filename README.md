# Индивидуальная работа

Этот проект представляет собой веб-приложение для продажи изделий ручной работы с молдавской тематикой. Реализован с использованием фреймворка Laravel.

## Установка и запуск

### Требования
- PHP >= 8.1
- Composer
- Node.js и npm
- SQLite или другая СУБД на выбор

### Установка
1. **Клонирование репозитория**:
   ```sh
   git clone https://github.com/Salam4ik666/inividualkaLaravel
   cd Individual2
   ```

2. **Установка зависимостей**:
   - PHP:
     ```sh
     composer install
     ```
   - JavaScript:
     ```sh
     npm install
     ```

3. **Настройка конфигурации**:
   ```sh
   cp .env.example .env
   ```

4. **Миграции и наполнение базы данных**:
   ```sh
   php artisan migrate --seed
   ```
   *(При необходимости можно использовать SQL-команды из `out.sql` для дополнительного заполнения базы.)*

5. **Сборка фронтенда**:
   ```sh
   npm run dev
   ```

6. **Запуск локального сервера**:
   ```sh
   php artisan serve
   ```

## Доступ к приложению

Открыть в браузере: [http://localhost:8000](http://localhost:8000)

**Данные для входа администратора:**
- **Email**: `123@mail.ru`
- **Пароль**: `12345678`

## Возможные проблемы и решения

- **Если не загружаются стили**:
  ```sh
  npm install
  npm run dev
  ```

- **Очистка кэша в случае ошибок**:
  ```sh
  php artisan config:clear
  php artisan cache:clear
  php artisan view:clear
