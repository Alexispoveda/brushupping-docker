FROM python:3.6-alpine
ENV PYTHONUNBUFFERED=1
WORKDIR /code
COPY . /code/
RUN python -m pip install --upgrade pip
RUN pip install -r requirements.txt
