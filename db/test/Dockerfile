FROM quay.io/bitnami/python:3.8.6-prod-debian-10-r81

WORKDIR /code

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY db_test.py .

CMD ["python", "db_test.py","0.0.0.0", "30004"]