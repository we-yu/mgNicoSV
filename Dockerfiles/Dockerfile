# Image select
FROM python:3.7-alpine3.7

ARG project_dir=/app/
WORKDIR $project_dir

RUN apk --no-cache add --virtual=addpacks curl vim
RUN apk del addpacks
RUN apk info

RUN pip install --upgrade pip
RUN pip install mysql-connector-python \
                pymongo \
                python-dotenv \
                requests \
                bs4
# execute at "docker run"
#CMD ["python", "frame_app.py"]
# ABCDEF
