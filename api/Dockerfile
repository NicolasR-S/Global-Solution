# Use a imagem base para a API
FROM node:14

# Defina o diretório de trabalho dentro do contêiner
WORKDIR /usr/src/app

# Copie o package.json e o package-lock.json para o diretório de trabalho
COPY package*.json ./

# Instale as dependências da API
RUN npm install

RUN yarn add express nodemon mysql cors

# Copie todo o código fonte da API para o diretório de trabalho
COPY . .

# Exponha a porta da API
EXPOSE 8080

# Inicie a API quando o contêiner for iniciado
CMD [ "npm", "start" ]
