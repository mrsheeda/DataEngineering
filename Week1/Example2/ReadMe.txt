FROM python:3.9: Sets the base image to the official Python 3.9 image.

RUN pip install pandas: Executes the command pip install pandas during the image build process, installing the pandas library into the image.

WORKDIR /app: Sets the working directory inside the container to /app, which will be the directory used for subsequent commands.

COPY pipeline.py pipeline.py: Copies the file pipeline.py from the build context to the /app directory inside the container.

ENTRYPOINT [ "bash" ]: Specifies that the default command to run when a container is created from the image is bash, which launches a bash shell.


docker build -t myimage: To build an image from this Dockerfile, 

docker run -it myimage: Once the image is successfully built, you can run a container from it by executing: