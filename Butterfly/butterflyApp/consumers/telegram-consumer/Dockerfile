# Base image
FROM python:3.7-slim

# Working directory
WORKDIR ./telegram-consumer

# Copy files into the container
COPY ./consumers/telegram-consumer .
COPY ./consumers/consumer.py ./consumers/
COPY ./consumers/__init__.py ./consumers/
COPY ./mongodb ./mongodb

# Install dependencies
RUN pip3 install -r requirements.txt

CMD python3 -m telegram
