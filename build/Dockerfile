FROM python:3.10-alpine

WORKDIR /app

<<<<<<< HEAD
COPY app/requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY app/*.py .
=======
COPY ./app/requirements.txt .
RUN --mount=type=cache,target=/root/.cache/pip \
    pip3 install -r requirements.txt

COPY . /app
>>>>>>> refs/remotes/origin/main

EXPOSE 8000

CMD ["python3", "app.py"]

