FROM python:3.7

RUN mkdir /app

RUN pip install numpy

ADD ./* $HOME/app/

WORKDIR /app/model/

CMD ["python", "model.py"]