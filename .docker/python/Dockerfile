FROM python:3.7.5-slim
WORKDIR /usr/src/app

RUN python -m pip install \
        parse \
        realpython-reader

RUN pip3 install kafka-python
COPY ./../producer-py/producer.py .
CMD ["python", "producer.py"]