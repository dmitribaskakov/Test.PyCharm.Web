# Test.PyCharm.Web
Test WEB Project in Python into PyCharm

#Обновление зависимостей

pip install -r requirements.txt

#Команды для докера:

docker build -t test.pycharm.web .

docker images

docker ps -a

docker rm $(docker ps -a -q)

docker run --name hello --rm test.pycharm.web


