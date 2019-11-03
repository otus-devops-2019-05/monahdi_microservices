FROM python:3.6.0-alpine
RUN apk add --update gcc python python-dev py-pip build-base

WORKDIR /app
ADD . /app

RUN pip install -r /app/requirements.txt

ENV POST_DATABASE_HOST post_db
ENV POST_DATABASE posts

ENTRYPOINT ["python3", "post_app.py"]
