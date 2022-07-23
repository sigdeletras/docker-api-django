# docker-api-django

## build the image by running

```
docker-compose build
```

## Create and Configure Django Project

```
docker-compose run --rm app sh -c "django-admin startproject app ."
```

## Crea modelo create model

```
docker-compose run --rm app sh -c "python manage.py startapp core"
```
```
docker-compose up
```

## Configure app for Deployment

docker-compose -f docker-compose-deploy.yml down --volumes
docker-compose -f docker-compose-deploy.yml build
docker-compose -f docker-compose-deploy.yml up

docker-compose -f docker-compose-deploy.yml run --rm app sh -c "python manage.py createsuperuser"