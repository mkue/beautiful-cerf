FROM python:3.7

COPY ./app /app

COPY requirements.txt /requirements.txt
RUN pip install --upgrade pip
RUN pip install -r /requirements.txt

ENV FLASK_APP app.py

WORKDIR /app

ENTRYPOINT [ "uvicorn" ]
CMD ["app:app", "--host", "0.0.0.0"]