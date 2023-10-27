FROM registry.access.redhat.com/ubi8/python-38

WORKDIR /app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY app.py .

EXPOSE 8080

# CMD [ "python3", "/app/app.py" ]
CMD python /app/app.py runserver 0.0.0.0:8080
