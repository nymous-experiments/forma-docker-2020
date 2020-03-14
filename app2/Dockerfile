FROM python:3-slim

EXPOSE 8000

COPY requirements.txt ./
RUN pip install -r requirements.txt

COPY main.py ./

CMD uvicorn mon_api.main:app --host 0.0.0.0
