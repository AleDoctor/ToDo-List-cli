# Lista de Tarefas (To-Do List) em Python + SQLite

Aplicação de linha de comando (CLI) para gerenciar tarefas, desenvolvida em
Python com persistência de dados em um banco SQLite.

## Funcionalidades

- Adicionar tarefa
- Listar tarefas (mostrando o que já foi concluído)
- Editar o título de uma tarefa
- Marcar tarefa como concluída
- Excluir tarefa

## Tecnologias utilizadas

- **Python 3**
- **SQLite** (biblioteca `sqlite3`, nativa do Python) para persistência dos dados

## Estrutura do projeto

```
todo-list-cli/
├── main.py         # Interface de linha de comando (menu e interação com o usuário)
├── database.py     # Camada de acesso ao banco de dados (todas as queries SQL)
└── README.md
```

O projeto separa a lógica de banco de dados (`database.py`) da lógica de
interface (`main.py`). Essa separação facilita manutenção e deixa claro
onde cada responsabilidade do sistema está.

## Como executar

```bash
python3 main.py
```

O banco de dados (`tarefas.db`) é criado automaticamente na primeira execução.

## Possíveis melhorias futuras

- Adicionar datas de vencimento nas tarefas
- Criar categorias/prioridades
- Migrar a interface para uma versão web
