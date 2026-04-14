# Django Task Manager API

Небольшой backend-проект под hh и junior/backend вакансии.

## Что реализовано
- регистрация пользователя
- JWT-аутентификация
- CRUD для задач
- фильтрация задач по статусу
- API на Django REST Framework

## Стек
- Python
- Django
- Django REST Framework
- SimpleJWT
- SQLite

## Запуск

```bash
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Открыть:
- API: `http://127.0.0.1:8000/api/tasks/`
- admin: `http://127.0.0.1:8000/admin/`

## Основные endpoints

### Регистрация
`POST /api/auth/register/`

```json
{
  "username": "ivan",
  "password": "StrongPass123",
  "email": "ivan@example.com"
}
```

### Получить JWT
`POST /api/auth/token/`

```json
{
  "username": "ivan",
  "password": "StrongPass123"
}
```

### Работа с задачами
- `GET /api/tasks/`
- `POST /api/tasks/`
- `GET /api/tasks/<id>/`
- `PATCH /api/tasks/<id>/`
- `DELETE /api/tasks/<id>/`

Пример создания задачи:
```json
{
  "title": "Сделать API",
  "description": "Подготовить pet-project",
  "status": "in_progress"
}
```

## Как описать в резюме

**Task Manager API (Python, Django, DRF)**
- разработал REST API для управления задачами
- реализовал регистрацию пользователей и JWT-аутентификацию
- реализовал CRUD-операции и фильтрацию данных
- работал с бизнес-логикой и структурой backend-приложения
