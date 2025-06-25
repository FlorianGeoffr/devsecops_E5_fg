FROM python:3.14.0b3-slim-bookworm
RUN apt-get update && apt-get upgrade -y && apt-get clean
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY app.py .
CMD ["python", "app.py"]
