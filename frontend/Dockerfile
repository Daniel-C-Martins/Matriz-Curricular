# Usar uma imagem base com Node.js
FROM node:18-slim

WORKDIR /app

# Instalar pnpm globalmente
RUN npm install -g pnpm

# Copiar package.json e pnpm-lock.yaml para o contêiner
COPY package.json pnpm-lock.yaml ./

# Instalar as dependências com pnpm (isso instalará o Vite também)
RUN pnpm install

# Copiar o restante dos arquivos para o contêiner
COPY . .

# Expor a porta 3000 para o frontend
EXPOSE 3000

# Rodar o frontend com pnpm
CMD ["pnpm", "dev"]