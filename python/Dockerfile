FROM arm32v6/python:3-alpine

WORKDIR /usr/src/app

COPY . .

# Install Python3 & dependencies.
RUN apk update && \
    apk upgrade && \
    apk add --no-cache gcc musl-dev linux-headers && \
    pip3 install -r requirements.txt

CMD ["python", "sensors.py"]