#Define a imagem
FROM node:14
#Define a pasta de trabalho
WORKDIR /app-node
#Copia os arquivos da pasta onde está o docker file para o diretório de trabalho app-node

COPY . .
#Arg só utilizado no tempo de build da imagem
ARG PORT_BUILD=6000
#Utilizada dentro do container
ENV PORT=$PORT_BUILD
EXPOSE $PORT_BUILD
# Instala as dependencias no momento em que o container está subindo
RUN npm install 
ENTRYPOINT npm start