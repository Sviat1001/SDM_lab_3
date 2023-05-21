FROM python:3.10-buster

WORKDIR /app

COPY . .

RUN pip install -r requirements/backend.in

ENV venv ./.venv

EXPOSE 8080

CMD ["uvicorn", "spaceship.main:app", "--host=0.0.0.0", "--port=8080"]