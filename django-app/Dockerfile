FROM python:3.9

WORKDIR /usr/src/app

COPY requirements.txt ./

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

RUN python -m django startproject myproject .

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
