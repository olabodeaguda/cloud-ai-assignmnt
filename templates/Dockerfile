FROM python:3.7
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
EXPOSE 9090
CMD gunicorn --workers=4 --bind 0.0.0.0:9090 app:app