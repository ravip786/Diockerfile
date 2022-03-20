
FROM ubuntu:latest 
WORKDIR /app
RUN apt-get update -y
RUN apt-get install -y python-dev
RUN  apt install -y python3-pip
COPY form.html /app/form.html
COPY requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt
COPY . /app   
CMD [ "python" , "./app.py" ]
EXPOSE 8000