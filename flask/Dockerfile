# syntax=docker/dockerfile:1
FROM alpine:3.21.3


# install app dependencies
RUN apk update && apk add --no-cache python3
RUN apk add --no-cache py3-flask

# install app
#COPY hello.py /

# configuracion final
ENV FLASK_APP=hello
EXPOSE 8000
CMD ["flask", "run", "--host", "0.0.0.0", "--port", "8000"]
