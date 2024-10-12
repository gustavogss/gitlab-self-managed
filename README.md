# Gitlab Self Managed
- Solução de controle de versão e gerenciamento de projetos usando gitlab com docker

## Como utilizar
- Instalar o docker e docker-compose
- Criar a rede gitlab no docker com o comando:
```
sudo docker network create gitlab
```
- baixar o projeto

- utilizar o comando para subir rodar o container:
```
docker-compose up -d
```
- Caso queira remover utilizar o comando:
```
docker-compose down
```
## Executando:

- Aplicação executa:
```
http://localhost:5050/
```
## Configurações:
- Configurar o usuário e senha:
1.  sudo docker exec -it gitlab grep 'Password:' /etc/gitlab/initial_root_password
2. sudo docker exec -it gitlab gitlab-rake "gitlab:password:reset"  
3. Definir um usuário e senha

