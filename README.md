# infra_sp2
### Описание
Проект для организации базы данных с отзывами на различные произведения искуства через api на основе RestAPI.
### Технологии
Python\
Django\
Django REST framework\
Docker
### Запуск проекта
- Перейти в папку ./infra/

```
cd infra/
```
- создайте файл .env и заполните его по подобию .env.template:
- Выполните команду:
```
docker-compose up -d
```
- Выполните команды:
```
docker-compose exec web python manage.py migrate
docker-compose exec web python manage.py collectstatic
```

### Примеры запросов
- Получение списка всех произведений
```
http://localhost:8000/api/v1/titles/
```
- Получение списка всех жанров
```
http://localhost:8000/api/v1/genres/
```
- Получение списка всех категорий
```
http://localhost:8000/api/v1/categories/
```
- Получение списка всех отзывов на произведение
```
http://localhost:8000/api/v1/titles/{title_id}/reviews/
```
- Вся Информация
```
http://localhost:8000/redoc/
```
### Авторы
- [Иван](https://github.com/AkuLinker/ "GitHub аккаунт")
