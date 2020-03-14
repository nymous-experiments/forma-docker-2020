FROM python:3-slim

EXPOSE 8000

WORKDIR /app

COPY requirements.txt ./
RUN pip install -r requirements.txt

COPY mon_api ./mon_api

CMD uvicorn mon_api.main:app --host 0.0.0.0
