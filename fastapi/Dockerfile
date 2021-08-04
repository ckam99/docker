FROM python:3.8-alpine

WORKDIR /app

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . .

EXPOSE 5001

# CMD ["python", "run.py"]

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "5001"]