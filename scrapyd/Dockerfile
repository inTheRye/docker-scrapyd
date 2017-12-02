FROM harrisbaird/scrapyd:py3

RUN mkdir /etc/scrapyd/
COPY ./config/scrapyd.conf /etc/scrapyd/scrapyd.conf

RUN mkdir /app
WORKDIR /app

COPY ./app /app
RUN pip3 install -r /app/requirements.txt

RUN scrapyd
