# django-api

Recipes API built with Python and Django

## Docker

The app is running inside the Docker container, so to be able to use the app you need the Docker to be installed in your system.

To start the server use:
`docker-compose up`

To stop the server use:
`Control + C` keys

To remove container from the Docker use:
`docker-compose down`

To build or re-build the Docker container use:
`docker-compose build`

To create new app use:
`docker-compose run --rm app sh -c "python manage.py startapp appname"`

## Tests

To run tests use this command:
`docker-compose run --rm app sh -c "python manage.py test"`

## Lint

To run linting use this command:
`docker-compose run --rm app sh -c "flake8"`

## API

To view the API docs in the browser go to http://localhost:8000/api/docs/#/

## Database

To generate new database migration files use this command:
`docker-compose run --rm app sh -c "python manage.py makemigrations"`

To apply all migrations to the database use this command:
`docker-compose run --rm app sh -c "python manage.py migrate"`
