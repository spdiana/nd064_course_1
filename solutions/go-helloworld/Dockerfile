FROM python:2.7
# set a key-value label for the Docker image
LABEL maintainer=""
# copy files from the host to the container filesystem.
# For example, all the files in the current directory
# to the  `/app` directory in the container
COPY . /techtrends
#  defines the working directory within the container
WORKDIR /app
# run commands within the container.
# For example, invoke a pip command
# to install dependencies defined in the requirements.txt file.
RUN pip install -r requirements.txt
# provide a command to run on container start.
# For example, start the `app.py` application.
CMD python init_db.py ; python app.py
#CMD [ "python", "app.py" ]

EXPOSE 3111


