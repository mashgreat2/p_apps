release: python manage.py migrate
web: gunicorn p_apps.wsgi --log-file -
worker: celery -A p_apps worker -l debug --app=p_apps.celery