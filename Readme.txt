create the first user using
docker-compose exec broker mosquitto_passwd -c /mosquitto/conf/mosquitto.passwd mosquitto


You can optionally create more users using the -b (batch) flag instead of -c , supplying the password on the command line:
docker-compose exec mosquitto mosquitto_passwd -b /mosquitto/conf/mosquitto.passwd seconduser shoaCh3ohnokeathal6eeH2marei2o


Now start mosquitto using
docker-compose up

docker exec -it mosquitto sh
suscripcion a Topico
mosquitto_sub -d -h localhost -p 1883 -t "casa/living"

Envio a Topico (en otra consola)
mosquitto_pub -d -h localhost -p 1883 -t "casa/living" -m "Encender Luz"


git init
git remote set-url origin https://github.com/fsachi/iot.git
git remote add . https://github.com/fsachi/iot.git
git add .
git commit -a
git commit -am "Initial  Commit"
git push origin

