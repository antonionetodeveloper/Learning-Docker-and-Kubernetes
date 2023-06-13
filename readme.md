# Aprendendo a usar o docker e o kubernetes

## Comandos básicos
    * `docker ps` - ve containers que estão rodando.
    * `docker ps -a` - ve todos os containers disponiveis.
    * `docker run` - roda um container.
    * `docker run -p 8080:80 container` redireciona a porta "80" do container para a porta "8080" da máquina.
    * `docker exec (ID/Name do container) (comando)` executa um comando no container
    * `docker run -p 8080:80 -v (src do computador):(src do container) nginx` - compartilha informações do computador com o container
    * `docker build -t (usuario do dockerHub)/(nome da imagem):latest (local do arquivo Dockerfile)` - compila um Dockerfile (que tem uma imagem) localmente em um container
    * `docker push (usuario do dockerhub)/(nome da imagem)` - publica uma imagem no dockerHub (é necessario logar antes)
    * `docker login` - faz o login
    * `docker logout` - faz o logout

### Docker compose
    * `docker compose up` - sobe as configs do arquivo "docker-compose"
    * `docker compose up -d` - roda em modo de desenvolvimento e em background (certifique-se de ter o parametro "volume" para salvar localmente e no container os arquivos)
    * `docker compose down` - mata todas as configurações do "docker compose up -d"


## Básico de kubernetes
em aprendizado...