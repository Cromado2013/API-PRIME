#### Desafio de Projeto Concluído

**Objetivo:**  
Neste projeto, você aplicou os conhecimentos adquiridos no módulo de API e Entity Framework do Croma 2013 para desenvolver um sistema gerenciador de tarefas.

**Contexto:**  
O sistema permite a organização eficiente das tarefas diárias, oferecendo uma lista interativa para gerenciar suas atividades.

**Requisitos Implementados:**  
A aplicação possui funcionalidades de CRUD (Criar, Ler, Atualizar e Deletar) para os registros de tarefas. Você optou por implementar uma Web API, que atende aos requisitos estabelecidos.

**Classe Principal:**  
A classe `Tarefa` foi criada com base no diagrama fornecido.

**Banco de Dados:**  
A migration necessária foi gerada e aplicada para atualizar o banco de dados com as novas configurações.

### Métodos Implementados

Utilizando Swagger para documentar a API, os seguintes métodos foram implementados:

| Verbo | Endpoint                       | Parâmetro | Body                |
|-------|--------------------------------|-----------|---------------------|
| GET   | /Tarefa/{id}                  | id        | N/A                 |
| PUT   | /Tarefa/{id}                  | id        | Schema Tarefa       |
| DELETE| /Tarefa/{id}                  | id        | N/A                 |
| GET   | /Tarefa/ObterTodos            | N/A       | N/A                 |
| GET   | /Tarefa/ObterPorTitulo        | titulo    | N/A                 |
| GET   | /Tarefa/ObterPorData          | data      | N/A                 |
| GET   | /Tarefa/ObterPorStatus        | status    | N/A                 |
| POST  | /Tarefa                       | N/A       | Schema Tarefa       |

**Schema (Model) da Tarefa:**  
A estrutura da tarefa foi definida como segue:

```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pendente"
}
```

### Conclusão

O projeto foi finalizado com sucesso, implementando todas as funcionalidades necessárias. O código está completo e funcional, conforme as diretrizes estabelecidas. 
