# Especifica a imagem base
FROM node:14

# Define o diretório de trabalho no contêiner
WORKDIR /usr/src/app

# Copia o arquivo package.json e package-lock.json (se disponível)
COPY package*.json ./

# Limpa o cache do npm
RUN npm cache clean --force

# Instala as dependências do projeto
RUN npm install

# Copia os arquivos do projeto para o contêiner
COPY . .

# Expõe a porta que o servidor usará
EXPOSE 3001

# Comando para iniciar o servidor
CMD ["npm", "start"]
