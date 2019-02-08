FROM fedora:28
COPY requirements.txt /op2/
WORKDIR /op2/
EXPOSE 8040
RUN dnf -y install python-pip
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
COPY . /op2/
ENTRYPOINT ./server.py -p 8040 -t -d config