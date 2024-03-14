# Instruções para Configurar o Projeto Docker React
## Pré-requisitos
### Antes de começar, você vai precisar ter instalado em sua máquina o  [Docker Desktop](https://www.docker.com/products/docker-desktop/).

### Além disto é bom ter um editor para trabalhar com o código como [VS Code](https://code.visualstudio.com/).

Siga os passos abaixo para clonar o repositório, entrar no diretório e iniciar o Docker:

### 1. **Clonar o Repositório:**
Abra o terminal e execute o seguinte comando para clonar o repositório:
```bash
git clone https://github.com/jessicaosilva/docker-react.git
```

### 2. **Entrar no Repositório:**
No terminal, execute o seguinte comando para mudar de pasta e entrar no projeto clonado:
```bash
cd docker-react
```

### 3. **Clonar o Repositório do Projeto React Frontend:**
Abra o terminal e execute o seguinte comando para clonar o repositório do projeto em react:
```bash
git clone https://github.com/jessicaosilva/front-app.git
```

### 4. **Clonar o Repositório do Projeto React Backend:**
Abra o terminal e execute o seguinte comando para clonar o repositório do projeto em react:
```bash
git clone https://github.com/jessicaosilva/back-app.git
```

### 5. **Build:**
Execute o seguinte comando para construir os serviços especificados no arquivo `docker-compose.yml`:
```bash
docker-compose build
```

### 6. **Iniciar o Docker Compose:**
Execute o seguinte comando para iniciar o Docker Compose e levantar os serviços em segundo plano:
```bash
docker-compose up -d
```

### Agora você tem dois ambientes de desenvolvimento React

#### .front-app/ - Projeto destinado a parte Frontend
#### .back-app/ - Projeto destinado a parte Backend

### 7. **Iniciar a aplicação Frontend:**
Abra a pasta piloto no seu editor de texto favorito.

```bash
docker-compose exec frontend npm start
```

ou 

```bash
docker exec -it docker-react-frontend-1 npm start
```

### 8. **Iniciar a aplicação Backend:**

Abra a pasta piloto no seu editor de texto favorito.
```bash
docker-compose exec backend npm start
```
ou 

```bash
docker exec -it docker-react-backend-1 npm start
```
Ambiente disponível em:
```bash
http://localhost:3001/
```

## Pronto!
