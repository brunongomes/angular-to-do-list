# Lista de Tarefas em Angular

Este projeto é uma aplicação básica de uma lista de tarefas, desenvolvida como exemplo de um CRUD (Create, Read, Update, Delete). Ele utiliza o `json-server` para simular um banco de dados local.

## Funcionalidades
- **Adicionar** novas tarefas.
- **Listar** todas as tarefas.
- **Marcar/Desmarcar** tarefas como concluídas (alteração de status).
- **Remover** tarefas.

> **Nota:** Não é possível editar o conteúdo das tarefas diretamente, apenas alterar o status de "concluído" ou "não concluído". Ao clicar duas vezes em uma tarefa, ela será marcada como concluída (fica destacada em verde).

## Tecnologias Utilizadas
- **Angular**: Para construir a interface do usuário.
- **json-server**: Para simular o backend e fornecer uma API RESTful simples.
- **JSON**: Armazena os dados localmente no arquivo `db.json`.

## Pré-requisitos
- **Node.js** (v14+)
- **Angular CLI** (v12+)
- **json-server** (instalado globalmente ou via `npx`)

## Como Executar o Projeto

1. **Clone o repositório**:

   ```bash
   git clone https://github.com/usuario/nome-do-repositorio.git
   cd nome-do-repositorio
   ```

2. **Instale as dependências**:

   ```bash
   npm install
   ```

3. **Inicie o servidor de desenvolvimento Angular**:

   ```bash
   ng serve
   ```

4. **Inicie o servidor JSON**:

   O `json-server` irá criar automaticamente o arquivo `db.json` na raiz do projeto para armazenar as tarefas. Para iniciar o servidor que simula a API:

   ```bash
   npx json-server --watch db.json
   ```

## Utilizando o Projeto
Após executar os servidores, você poderá acessar a aplicação pelo navegador:

- Acesse a interface da lista de tarefas em [http://localhost:4200](http://localhost:4200)
- A API simulada estará disponível em [http://localhost:3000](http://localhost:3000)

## Estrutura de Arquivos

```
.
├── src/
│   └── ...
├── db.json          # Arquivo gerado pelo json-server para armazenar as tarefas
├── angular.json     # Configurações do Angular
├── package.json     # Dependências do projeto
└── README.md        # Este arquivo
```

## Considerações Finais

Este é um projeto simples para praticar a criação de uma aplicação CRUD em Angular e usar o `json-server` como backend falso. Sinta-se à vontade para contribuir e sugerir melhorias.
