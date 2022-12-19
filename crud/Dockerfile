FROM python:3.9

COPY ./stocks_products/requirements.txt /src/stocks_products/requirements.txt
RUN pip3 install -r /src/stocks_products/requirements.txt
COPY . /src
EXPOSE 8000

WORKDIR src

CMD ["python3", "stocks_products/manage.py", "runserver", "0.0.0.0:8000"]