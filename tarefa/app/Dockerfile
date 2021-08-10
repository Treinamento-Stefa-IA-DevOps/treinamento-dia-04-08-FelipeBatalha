
#FROM python:3.8-slim
FROM centos/python-36-centos7

COPY . /app

WORKDIR /app

RUN pip install -r requirements.txt
# requerimento para rodar o flask run
ENV MAIN=main.py  

CMD ["uvicorn","main:app","--host","0.0.0.0","--port","80","--reload"]
