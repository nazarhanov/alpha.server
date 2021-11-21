FROM ghcr.io/nazarhanov/alpha:latest 

CMD python3 manage.py collectstatic --noinput \ 
 && python3 manage.py migrate \ 
 && gunicorn alpha.wsgi:application --bind 0.0.0.0:8000
