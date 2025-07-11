#Sets the base image for your Docker image.This image comes with Python pre-installed.It gives you a reliable Python environment to run your app in.
FROM python:3.8 

#Tells Docker that the container will listen on port 8080 at runtime.
EXPOSE 8080 

#Sets the working directory inside the container to /app.
WORKDIR /app

#Copies everything in your current directory (on your host machine) into the /app directory inside the container.
COPY . ./

#Installs all Python dependencies listed in the requirements.txt file using pip.
RUN pip install -r requirements.txt

#Specifies the default command to run when the container starts.
CMD ["python", "app.py"]


