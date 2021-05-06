# 🟢 SOLUÇÃO EM DJANGO

## Projeto recipe-app-api-proxy

  > Proxy para aplicação recipe-app-api, com pipeline no Gitlab

## Usage

### Environment Variables

- `LISTEN_PORT` - Port to listen on (default: `8000`)
- `APP_HOST` - Hostname of the app to forward requests to (default: `app`)
- `APP_PORT` - Port of the app to forward requests to (default: `9000`)

### Running local machine

´´´shell
  $ cd /receipe-app-api-proxy
  $ docker build -t proxy .
  $ cd ../recipe-app-api
  $ docker-compose -f docker-compose-proxy.yml up
´´´

- Test: <http://localhost:8000/admin/>
