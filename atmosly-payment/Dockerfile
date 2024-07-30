FROM python:3.9

EXPOSE 8080
USER root

ENV INSTANA_SERVICE_NAME=payment

WORKDIR /app

COPY atmosly-payment/requirements.txt /app/

RUN pip install -r requirements.txt

COPY atmosly-payment/*.py /app/
COPY atmosly-payment/payment.ini /app/

#CMD ["python", "payment.py"]
CMD ["uwsgi", "--ini", "payment.ini"]

