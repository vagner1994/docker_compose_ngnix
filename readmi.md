Passo 1: Instale o Docker
Antes de tudo, você precisa ter o Docker instalado no seu computador. O Docker é uma ferramenta que permite criar e executar contêineres. Você pode baixá-lo e instalá-lo em Docker Desktop.


2. Crie um diretório chamado `C:\trabalho` em sua máquina local, se ainda não existir.

 

3. Abra um editor de texto e crie um arquivo chamado `docker-compose.yml` com o seguinte conteúdo:

version: '3'

 

services:
  nginx:
    image: nginx:latest
    container_name: servidor-nginx
    ports:
      - "8920:80"
    volumes:
      - C:\trabalho:/usr/share/nginx/html

 

4. Salve o arquivo docker-compose.yml no mesmo diretório onde você possui o arquivo index.html.

 

5. Abra o terminal ou prompt de comando e navegue até o diretório onde estão os arquivos index.html e docker-compose.yml.

Passo 4: Abra um terminal do visual studio
Insira o comanado 
docker compose up -d
deixa carregar o codigo

Passo5: Abra o navegador
Na barra de endereço digite http://localhost/index.html
a pagina sera exibida

