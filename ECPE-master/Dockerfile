FROM python:2.7-jessie
USER root

RUN mkdir /aspect_extract2
WORKDIR /aspect_extract2
ADD ./ /aspect_extract2/

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
    build-essential \
    python-pip \
    tor \
    vim \
    && apt-get clean


RUN pip install nltk
RUN pip install keras==2.2
RUN pip install numpy==1.15
RUN pip install tensorflow-gpu==1.8.0
RUN pip install gensim==3.5


EXPOSE 8881
