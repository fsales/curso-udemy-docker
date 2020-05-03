## Docker - curso Udemy

#### Dicas Docker

Inicializar contêiner
```sh
$ docker run  -it ubuntu:19.04 /bin/bash
```

Sair contêiner
```sh
$ exit
```

Parar contêiner
```sh
$ docker stop {id_container}
```

Iniciar contêiner
```sh
$ docker start {id_container}
```

Attach contêiner
```sh
$ docker attach {id_container}
```

Sair sem parar contêiner
```sh
$ ctrl + p + q
```

Reiniciar contêiner
```sh
$ docker restart {id_container}
```

Listar contêiner em execução
```sh
$ docker ps
```

Listar último contêiner em que foi executado
```sh
$ docker ps -l
```

Listar detalhes sobre o docker
```sh
$ docker info
```

Remover contêiner
```sh
$ docker rm {id_container}
```

Log contêiner
```sh
$ docker logs {id_container}
```

Listar docker info
```sh
$ docker inspect {id_container}
```

Acessar contêiner
```sh
$ docker exec -it {id_container}
```
Listar imagens
```sh
$docker images
```  

#### Dockerfile
Exemplo disponível em test-dockerfile/Dockerfile

Criar contêiner
```sh
$ docker build -t helloword:0.1.0 ./test-dockerfile
```
```sh
$ docker build -t="build1" .
```

Histórico alteração
```sh
$docker history helloword:0.1.0 
```  

#### Docker Registries
Criar tag antes de enviar imagem para docker hub 

Enviar imagem para o docker hub
```sh
$docker tag {id_container} {usuario_docker}/helloword:0.1.0
```   

Logar Docker Hub

```sh
$docker login docker.io
```

Enviar imagem Docker Hub

```sh
$docker push {id_container} {usuario_docker}/helloword:0.1.0
```

Executar servidor
```sh
docker run -d -p 80:80 webserver 
```

#### Docker Compose
Criar o arquivo docker-compose.yml

Iniciar contêiner
```sh
docker-compose up -d
```

Para contêiner
```sh
docker-compose down
```

Listar contêiner
```sh
docker-compose ps
```

