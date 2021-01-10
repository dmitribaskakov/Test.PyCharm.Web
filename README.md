# Test.PyCharm.Web
Test WEB Project in Python into PyCharm

#Обновление зависимостей

pip install -r requirements.txt

#Команды для докера:

docker build -t test.pycharm.web .

docker images

docker ps -a

docker rm $(docker ps -a -q)

docker run --detach --rm --name web --publish 8080:8080 --env TZ=Asia/Novosibirsk test.pycharm.web

docker run --detach --rm --name web --publish 8080:8080 --env TZ=Asia/Novosibirsk --volume C:\Projects\Test.PyCharm.Web\resources\:/usr/src/app/resources/ test.pycharm.web

docker volume ls

docker volume create web

docker run --detach --rm --name web --publish 8080:8080 --env TZ=Asia/Novosibirsk --volume web:/usr/src/app/resources/ test.pycharm.web





