from python:3.11-slim

WORKDIR /app

#Install dependency
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

#Copy source code
COPY main.py main.py

EXPOSE 8000

CMD ["unicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]