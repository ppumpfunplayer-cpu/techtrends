FROM python:3.8

WORKDIR /app

COPY . .

RUN pip install -r requirements.txt

RUN python init_db.py

ENV FLASK_APP=app.py 

EXPOSE 3111

CMD ["python", "-m", "flask", "run", "--host=0.0.0.0", "--port=3111"]