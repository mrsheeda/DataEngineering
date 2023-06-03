# in this example, I will pass argument to docker container, rather going inside and run the python code.

FROM python:3.9

RUN pip install pandas

WORKDIR /app

COPY pipeline.py pipeline.py

ENTRYPOINT [ "python","pipeline.py" ]


