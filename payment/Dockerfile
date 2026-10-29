FROM python:3.9
WORKDIR /app
COPY requirements.txt .
COPY *.py .
COPY payment.ini .
RUN pip3 install -r requirements.txt
EXPOSE 8080
# ExecStart=/bin/java -jar /app/shipping.jar
CMD ["uwsgi", "--ini", "payment.ini"]