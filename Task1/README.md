# Команды для запуска
Находясь в директории Task1 выполните:
docker build . --tag=my_app:1.0
docker run -d -p 8000:80 my_app:1.0