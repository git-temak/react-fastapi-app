FROM python:3.10

WORKDIR /app

COPY . /app

# Create and activate a virtual environment
RUN pip install -r requirements.txt

EXPOSE 8000

ENV HNG_LESSON_DAY='day1' \
    HNG_API_ORIGINS='http://127.0.0.1:7000,http://localhost:7000,http://localhost:3000' \
    HNG_API_HOST='localhost' \
    HNG_API_PORT=8000

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]