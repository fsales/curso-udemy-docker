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

#### Dockerfile
Exemplo disponível em test-dockerfile/Dockerfile

Criar contêiner
```sh
$ docker build -t helloword:0.1.0 ./test-dockerfile
```

Histórico alteração
```sh
$docker history helloword:0.1.0 
```   