FROM python:3.9
EXPOSE 8000
RUN mkdir /app
WORKDIR /app
COPY ./requirements.txt ./requirements.txt
RUN pip install -r requirements.txt
COPY . .
RUN python manage.py makemigrations && python manage.py migrate
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
