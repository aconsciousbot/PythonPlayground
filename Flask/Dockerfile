FROM python:3.7.2-alpine

EXPOSE 8080
WORKDIR /usr/src/app
COPY . .

RUN pip install flask gunicorn


CMD ["gunicorn", "app:app", "-b", "0.0.0.0:8080", "--workers", "4", "--reload"]