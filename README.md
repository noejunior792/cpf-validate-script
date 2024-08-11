# CPF Validator API 📃

Uma API simples desenvolvida em Node.js para validar CPFs brasileiros. Este projeto permite que outras aplicações consumam esta API para verificar se um CPF é válido ou não.

## Funcionalidades ✨

- Validação de CPFs via API.
- Suporte a requisições POST com JSON.
- Respostas em formato JSON indicando se o CPF é válido.

## Tecnologias Utilizadas ⚙️

- Node.js
- Express

## Requisitos 🎓

- Node.js (versão 14.x ou superior)
- NPM (versão 6.x ou superior)

## Instalação 💀

1. Clone o repositório para a sua máquina local:

   ```bash
   git clone https://github.com/noejunior792/cpf-validator-api.git
   cd cpf-validator-api
   npm install
   npm start
   ```

## Como Usar 💻

### Endpoints

#### POST /api/cpf/validate

Este endpoint valida um CPF e retorna se ele é válido ou não:

- URL: /api/cpf/validate
- Método: POST
- Headers: Content-Type: application/json
- Body: JSON contendo o CPF a ser validado.

### Exemplo de requisição

```bash
curl -X POST http://localhost:3000/api/cpf/validate -H "Content-Type: application/json" -d '{"cpf": "12345678909"}'

```

### Exemplo de resposta

```bash
{
  "cpf": "12345678909",
  "isValid": false
}
```

## Contribuindo 🔥

Contribuições são bem-vindas! Por favor, envie um pull request ou abra uma issue para discutir mudanças que gostaria de fazer.