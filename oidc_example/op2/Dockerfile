FROM python:3.6
COPY requirements.txt /op2/
WORKDIR /op2/
EXPOSE 8040
RUN pip install -r requirements.txt
COPY . /op2/
ENTRYPOINT ./server.py -p 8040 -t -d config_simple.py
