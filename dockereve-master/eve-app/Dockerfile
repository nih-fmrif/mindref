FROM python:3.4-onbuild

WORKDIR /usr/src/app

ADD . /usr/src/app


RUN pip3 install -r requirements.txt
RUN pip3 install pytest
RUN cp /usr/src/app/*.cfg /usr/local/lib/python3.4/site-packages/eve/
RUN cat /usr/local/lib/python3.4/site-packages/eve/*.cfg
#RUN sed -i 's/\[scheme\]/\["https"\]/' /usr/local/lib/python3.4/site-packages/eve_swagger/objects.py

#EXPOSE 5000
#CMD ["python3", "server.py"]

