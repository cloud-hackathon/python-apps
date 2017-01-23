FROM python:3.6.0-alpine

ENV PYTHONUNBUFFERED 1
RUN mkdir /code
WORKDIR /code

COPY ./src/* /code/
RUN pip install -r requirements.txt

EXPOSE 8080
ENTRYPOINT ["python", "manage.py", "runserver", "8080"]
