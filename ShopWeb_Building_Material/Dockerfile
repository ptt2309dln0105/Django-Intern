FROM python:3
ENV PYTHONUNBUFFERED=1
WORKDIR /code
COPY requirements.txt /code/
RUN pip install -r requirements.txt
COPY . /code/

CMD python3 manage.py migrate
CMD python3 manage.py runserver 0.0.0.0:8000