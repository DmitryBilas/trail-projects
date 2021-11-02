FROM python:3.7


RUN mkdir -p /usr/src/app/
WORKDIR /usr/src/app/

COPY . /usr/src/app/
RUN pip install --no-cache-dir -r requirements.txt

# Проброс 8080 порта
# docker run --rm -p 8080:8080 web-hello-world
EXPOSE 8080

# Set timezone
# ENV TZ Europe/Moscow

CMD ["python", "app.py"]

# docker run --rm -p 8080:8080 -e TZ=Europe/Moscow web-hello-world