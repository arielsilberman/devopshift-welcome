FROM python:3.12-slim

WORKDIR /fe/src
ENV PYTHONDONTWRITEBYTECODE=1 \
    PYTHONUNBUFFERED=1

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .
EXPOSE 5002


CMD ["python", "src/main.py"]