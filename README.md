# email-worker-compose
Docker Envio de E-mails com Workers

![E-mails com workers](https://user-images.githubusercontent.com/47223292/123892449-ff4fa780-d930-11eb-93ab-261685ad6539.PNG)

docker-compose up

docker-compose ps

docker-compose exec db psql -U postgres -f ./scripts/check.sql

docker-compose exec db psql -U postgres -d email_sender -c 'select * from emails'

docker-compose down
