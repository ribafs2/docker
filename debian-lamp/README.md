# Docker debian devel

Esta imagem contém o LAMP (Debian, Apache, MariaDb e PHP 5.6, 7.4 ou 8.1)

Com dois CRUDs, um com mariadb e outro com sqlite

Os CRUDs usam PHP, PDO, paginação e bootstrap.

## Como usar

Execute

cp sample.env .env

Abra o .env e altere a gosto a versão do PHP

## Remover

Para garantir, caso queira remover todas as imagens e containers existentes:

Parar todos os containers rodando:

```bash
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
Remover todas as imagens
docker rmi $(docker images -a -q)
```
## Criar o container através da imagem
```bash
docker-compose up -d
```
Ao final
```bash
docker images
docker run -it nomeimagem
```
Executar:
```bash
start.sh - Se setou o .env para 56

start2.sh - Se setou o .env para 74 ou 81

source /root/.bashrc

ip a
```
Abra no desktop

http://172.17.0.2
