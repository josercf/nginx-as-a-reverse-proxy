# Dockerfile para API 1 (Duplicar e ajustar para API 2 e API 3 mudando a porta e a mensagem)
FROM node:14

# Cria um diretório de trabalho
WORKDIR /usr/src/app

# Instala as dependências do projeto
# O arquivo package.json E package-lock.json são copiados
COPY package*.json ./
RUN npm install

# Copia os arquivos do projeto
COPY . .

# Expõe a porta que o container vai escutar
EXPOSE 3002

# Comando para rodar a aplicação
CMD ["node", "server.js"]
