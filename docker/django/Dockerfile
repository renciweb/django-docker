FROM python:3.7

ENV PYTHONUNBUFFERED 1
ENV DJANGO_SECRET_KEY i#(2*)zt0x#@#c-@qq*d$6=3l_@ryw0tc=k!cwxwp&v2be_2tr

RUN apt-get update
RUN apt-get install -y --no-install-recommends apt-utils
RUN apt-get install -y nano

RUN mkdir /src
COPY ./src /src
WORKDIR /src

RUN pip install pipenv && pipenv install --system
