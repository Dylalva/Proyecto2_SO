FROM python:3.12-slim

WORKDIR /app

COPY requirements.txt .

RUN pip install --upgrade pip

RUN pip install --no-cache-dir -r requirements.txt


COPY . .

#ENV FLASK_APP=app.py
#ENV FLASK_ENV=development

EXPOSE 5001
CMD ["flask", "run", "--reload", "--host=0.0.0.0", "--port=5001"]