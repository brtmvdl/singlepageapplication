# Docker SPA

[![github/actions/workflow/status](https://img.shields.io/github/actions/workflow/status/brtmvdl/docker-spa/docker-push.yml)](https://img.shields.io/github/actions/workflow/status/brtmvdl/docker-spa/docker-push.yml) [![github/license](https://img.shields.io/github/license/brtmvdl/docker-spa)](https://img.shields.io/github/license/brtmvdl/docker-spa) [![github/stars](https://img.shields.io/github/stars/brtmvdl/docker-spa?style=social)](https://img.shields.io/github/stars/brtmvdl/antify?style=social)

Imagem Docker para facilitar a configuração de aplicações SPA

Veja mais em [hub.docker.com/r/tmvdl/spa](https://hub.docker.com/r/tmvdl/spa)

## Como usar

Instalar o [Docker](https://docs.docker.com/engine/install/).

### Uso 1

1. Criar um arquivo `docker-compose.yaml` na raiz do projeto com a imagem [tmvdl/spa](https://hub.docker.com/r/tmvdl/spa).

```yaml
# docker-compose.yaml
version: '3'

services:
  app:
    image: tmvdl/spa
    volumes:
      - .:/app
```

2. Subir o container para a construção do build

```bash
docker-compose up --build
```

### Uso 2

1. Executar como container do Docker

```sh
docker run -p 1220:80 tmvdl/spa
```

2. Abrir `localhost:1220` no browser

## License

[MIT](LICENSE)

## Update

Atualizado em 12/01/2022
