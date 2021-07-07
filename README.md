# email-worker-compose
Docker Envio de E-mails com Workers

![E-mails com workers](https://user-images.githubusercontent.com/47223292/123892964-e98eb200-d931-11eb-91aa-d5d478b00f37.PNG)

docker-compose up -d

docker-compose ps

docker-compose exec db psql -U postgres -f ./scripts/check.sql

docker-compose exec db psql -U postgres -d email_sender -c 'select * from emails'

docker-compose logs -f -t

docker-compose up -d --scale worker=3

docker-compose logs -f -t worker

docker-compose down
