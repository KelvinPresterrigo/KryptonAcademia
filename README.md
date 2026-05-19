# 🏋️ Krypton Academia — Sistema de Gestão de Academia

> Plataforma integrada de gestão de preparo físico e nutricional para academias.

---

## 📋 Sobre o Projeto

O **Krypton Academia** é um software de gestão voltado para academias de médio e grande porte, integrando o acompanhamento de treinos, nutrição e gestão de alunos em uma única plataforma. O sistema conecta donos de academia, personal trainers, nutricionistas e alunos com hierarquia de acesso definida por perfil.

---

## 🚀 Como Rodar o Projeto

### Pré-requisitos

Certifique-se de ter instalado em sua máquina:

- [npm](https://www.npmjs.com/) 
- [Node.js](https://nodejs.org/) 
- [Git](https://git-scm.com/)
- [MySQL Workbench](https://www.mysql.com/downloads/).

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/krypton-academia.git
cd krypton-academia
```

---

### 2. Configure as variáveis de ambiente

Crie um arquivo .env e preencha com suas configurações:
```
PORT=3000
NODE_ENV=development

# JWT
JWT_SECRET= 
JWT_EXPIRES_IN= 

# MySQL
DB_HOST=localhost
DB_PORT=3306 
DB_USER=root 
DB_PASSWORD= 
DB_NAME=academia_kripton

```

Copie o texto acime e cole no arquivo `.env` com as informações do seu ambiente:

# Configurações do servidor
PORT=3000 (A porta onde o servidor Node.js vai rodar )
NODE_ENV=development(Define o ambiente. Em development, erros são mais verbosos. Em production, o app otimiza performance e oculta detalhes de erro).

# Autenticação (JWT- JSON Web Token)
JWT_SECRET=*String para assinar o token!* (Chave secreta usada para assinar e validar tokens JWT (login/sessão). Se vazar, alguém pode forjar tokens de autenticação)
JWT_EXPIRES_IN=7d

# MySQL
DB_HOST=localhost(Endereço do servidor MySQL.)
DB_PORT=3306 (Porta padrão do MySQL)
DB_USER=root (Usuário do banco. root é o superusuário (ok em dev, evitar em produção))
DB_PASSWORD= (Senha do MySQL Workbench)
DB_NAME=academia_kripton (Nome do projeto)
---

### 3. Instale as dependências

Baixe o Express(https://expressjs.com/)
```
npm install 
npm install express
```
npm install nodemon (Opcional, para desenvolvimento com hot reload)
```
npm install nodemo
```
Para rodar o arquivo execute o:
```
npm run dev
```
ou
```
npm start
```
Se tudo estiver configurado corretamente ele ira rodar na porta localhost
> Servidor disponível em: `http://localhost:3000`
