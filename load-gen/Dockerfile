FROM python:3.9

# Some default values
ENV HOST="https://rb.test.atmosly.in/" \
    SILENT=0 \
    NUM_CLIENTS=1 \
    ERROR=0 \
    RUN_TIME=0
    

WORKDIR /load

COPY load-gen/requirements.txt /load/

RUN pip install -r requirements.txt

COPY load-gen/entrypoint.sh /load/
COPY load-gen/robot-shop.py /load/

CMD ["./entrypoint.sh"]

