# Configurando um Nginx Proxy Reverso com Docker
Este é um guia para configurar um Nginx Proxy Reverso usando Docker.

## Pré-requisitos
Antes de começar, você precisará ter o Docker instalado na sua máquina.

## Configurando o Proxy Reverso
Clone o repositório para a sua máquina:

```sh
gh repo clone eliezermachado/nginx-proxyreverso

```

## Adicionando certificados
Crie a estrutura de pasta para armazenar os certificados
```sh
mkdir /etc/certificados/
```
Adicione os arquivos de certificados(.crt, .key) dentro da pasta que acabamos de criar. o caminho dos arquivos deverão estar da seguinte maneira:
    /etc/certificados/meucertificado.crt
    /etc/certificados/meucertificado.key

## Executando docker 
Na raiz do projeto execute o docker compose para inicializar o proxy
```sh
docker compose up -d
```