FROM python:2.7.12

COPY requirements.txt /requirements.txt
RUN pip install -r requirements.txt

WORKDIR /app
COPY . ./
COPY docker/config.ini ./

VOLUME /books
VOLUME /db
VOLUME /log
VOLUME /main
CMD python cps.py
EXPOSE 8000
