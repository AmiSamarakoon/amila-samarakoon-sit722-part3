# Dockerfile for book_catalog microservice
FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

ENV DATABASE_URL = "postgresql://sit722_task3_user:DYCeLi20kuIvZ9kcnXKN2wWS2E92sqeu@dpg-crkjdou8ii6s7380oov0-a.oregon-postgres.render.com/sit722_task3"

EXPOSE 8000

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8000"]