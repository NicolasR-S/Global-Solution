# Use a imagem base para o frontend
FROM node:14

# Defina o diretório de trabalho dentro do contêiner
WORKDIR /usr/src/app

# Copie o package.json e o package-lock.json para o diretório de trabalho
COPY package*.json ./



# Instale as dependências do frontend
RUN npm install

RUN npm install react-toastify

RUN npm install styled-components

RUN npm install axios

RUN npm install react-icons



# Copie todo o código fonte do frontend para o diretório de trabalho
COPY . .

# Exponha a porta do frontend
EXPOSE 3000

# Inicie o frontend quando o contêiner for iniciado
CMD [ "npm", "start" ]
