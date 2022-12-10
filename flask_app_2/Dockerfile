FROM ubuntu:22.04
RUN apt-get update && apt-get install -y python3 python3-pip
RUN pip install flask==2.1.* redis
COPY hello.py /
ENV FLASK_APP=hello
ENTRYPOINT [ "python3" ]
CMD [ "hello.py" ]
#EXPOSE 5002
#CMD flask run --host 0.0.0.0 --port 5002