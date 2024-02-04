

# Buildar a aplicação:
cargo build --release

## ================
## DOCKER CONTAINER
## ================

# Construir um container:
docker build -t my-store-rust-api .

# Executar container:
docker run <CONTAINER_ID>
docker run -d -p 8080:8080 <CONTAINER_ID>

# Ver containers em execução:
docker ps
docker ps -s

# Listar containers:
docker ps -a

# Parar um container
docker stop <CONTAINER_ID> 

# Pausar e despausar um container:
docker pause <CONTAINER_ID>
docker unpause <CONTAINER_ID>

# Remover container:
docker rm <CONTAINER_ID>

# Ver mapeamento de portas em relação ao Host:
docker port <CONTAINER_ID>
docker run -d -p 8080:80 <IMAGE_ID>
Obs.: mapeia a porta 80 do container para a porta 8080 do Host

## =============
## DOCKER IMAGES
## =============

# Executar imagem:
docker run -d <IMAGE_ID>

# Listar imagens:
docker images

# Remover imagem:
docker rmi <IMAGE_ID>