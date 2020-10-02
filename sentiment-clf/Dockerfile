FROM python
WORKDIR /project
ADD . /project
RUN apt update; apt-get -y install python3-matplotlib
RUN pip install -r requirements.txt
VOLUME /project/lib/models
CMD python build_model.py && python app.py