# docker-api-django

build the image by running

```
docker-compose build
```

Create and Configure Django Project

```
docker-compose run --rm app sh -c "django-admin startproject app ."
``

create model

docker-compose run --rm app sh -c "python manage.py startapp core"