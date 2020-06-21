FROM python:3.8

RUN pip install aiohttp gunicorn

COPY api.py /api.py

CMD gunicorn --worker-class aiohttp.GunicornWebWorker --workers 2 api:app
