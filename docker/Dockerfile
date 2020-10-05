FROM tiangolo/uwsgi-nginx-flask:python3.6

RUN mkdir /app/

COPY /pipeline/model/model.py /app/
COPY /pipeline/preprocessing/preprocessing.py /app/
COPY /pipeline/utils/utils.py /app/

RUN pip install numpy
RUN pip install random

WORKDIR /app/

CMD ["python", "/app/model/model.py"]

