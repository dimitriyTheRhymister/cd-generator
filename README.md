# Generator Service

Генерация экзаменационных вопросов на основе вакансий hh.ru.

## 🔧 Технологии
- Java 21
- Spring Boot 2.7.11
- PostgreSQL
- Liquibase
- Jsoup, Gson
- Eureka Client

## 📦 Порт
9903

## 🗄️ База данных
- Имя: cd_generator
- Пользователь: postgres
- Пароль: password

## 📚 API Endpoints

| Метод | URL | Описание |
|-------|-----|----------|
| GET | /exam/create/?url={link} | Генерация вопросов |
| GET | /statistic/get | Статистика вакансий |
| GET | /statistic/renew | Обновить статистику |
| POST | /statistic/create | Добавить ключевое слово |
| PUT | /statistic/update | Обновить ключевое слово |
| DELETE | /statistic/delete/{id} | Удалить ключевое слово |

## 🔗 Eureka
Регистрируется под именем generator

## 🚀 Запуск
```bash
mvn spring-boot:run