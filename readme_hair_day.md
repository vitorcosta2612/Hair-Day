# ✂️ Hair Day

> Sistema web intuitivo e moderno para agendamento de horários em salão de beleza e barbearia.

---

## 📌 Sobre o Projeto

O **Hair Day** é uma aplicação desenvolvida para otimizar o fluxo de atendimento em salões de beleza. Com ele, o cliente pode selecionar a data desejada, visualizar os períodos disponíveis (manhã, tarde e noite) e agendar um serviço de forma rápida. O sistema se comunica com uma API simulada para persistência dos dados e controle de horários indisponíveis.

Este projeto foca em boas práticas com **JavaScript Vanilla**, modularização de código, empacotamento com **Webpack** e automação via **npm/Node.js**.

---

## 🚀 Tecnologias Utilizadas

- **[JavaScript (ES6+)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript):** Lógica da aplicação, manipulação do DOM e requisições assíncronas (`fetch` / `async/await`).
- **[Node.js](https://nodejs.org/):** Ambiente de execução JavaScript para gerenciamento de ferramentas e build.
- **[npm](https://www.npmjs.com/):** Gerenciador de dependências e execução de scripts de desenvolvimento.
- **[Webpack](https://webpack.js.org/):** Empacotador de módulos (*bundler*), responsável por compilar, otimizar assets, carregar estilos e transpilar código com auxílio do Babel.
- **[JSON Server (API Mock)](https://github.com/typicode/json-server):** Simulação de uma REST API para operações de leitura, criação e exclusão de agendamentos.
- **[Day.js](https://day.js.org/):** Biblioteca para manipulação, validação e formatação de datas e horários.

---

## ✨ Funcionalidades

- [x] Seleção de data com filtro dinâmico de horários.
- [x] Exibição de horários divididos por períodos (Manhã, Tarde e Noite).
- [x] Validação em tempo real: bloqueio de horários passados ou já ocupados.
- [x] Criação de novo agendamento com persistência via requisição `POST` na API.
- [x] Listagem em tempo real de agendamentos do dia selecionado.
- [x] Cancelamento/remoção de agendamentos com requisição `DELETE`.

---
---

## 🛠️ Como Executar o Projeto

### Pré-requisitos

Certifique-se de ter o **[Node.js](https://nodejs.org/)** (versão 18+ recomendada) e o **npm** instalados em sua máquina.

### 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/hair-day.git
cd hair-day
```

### 2. Instalar as dependências

```bash
npm install
```

### 3. Iniciar o servidor da API (JSON Server)

Em um terminal, inicie a API simulada:

```bash
npm run server
```
> Por padrão, a API estará acessível em: `http://localhost:3333`

### 4. Iniciar a aplicação (Webpack Dev Server)

Em outro terminal, execute o servidor de desenvolvimento:

```bash
npm run dev
```
> A aplicação abrirá automaticamente no seu navegador padrão em: `http://localhost:3000` (ou porta configurada).

### 5. Gerar build para produção

Para compilar e minificar os arquivos finais na pasta `dist/`:

```bash
npm run build
```

---

## 📝 Scripts Disponíveis

| Comando | Descrição |
| :--- | :--- |
| `npm run dev` | Inicia o servidor de desenvolvimento Webpack com live reload. |
| `npm run build` | Empacota e otimiza os arquivos para produção na pasta `dist/`. |
| `npm run server` | Executa o `json-server` observando o arquivo `server.json`. |

---

## 📄 Licença

Este projeto está sob a licença [MIT](LICENSE).

---

Feito com 💜 para estudos e aprimoramento de habilidades no ecossistema JavaScript.