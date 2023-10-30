Alterar o nome de um projeto específico:
```
db.Project.updateOne(
    { _id: ObjectId("ID_do_Projeto_Aqui") },
    { $set: { "name": "Novo Nome do Projeto" } }
)
```


Atualizar a data de término de um projeto específico:
```
db.Project.updateOne(
    { _id: ObjectId("ID_do_Projeto_Aqui") },
    { $set: { "end_date": ISODate("NovaDataAqui") } }
)

```


Adicionar uma nova tarefa a um projeto específico:
```
db.Project.updateOne(
    { _id: ObjectId("ID_do_Projeto_Aqui") },
    { $push: { "tasks": {
        "title": "Nova Tarefa",
        "description": "Descrição da Nova Tarefa",
        "start_date": ISODate("DataDeInicioAqui"),
        "deadline_date": ISODate("DataDeLimiteAqui"),
        "priority": "Média",
        "status": "Pendente",
        "user": {
            "first_name": "NovoNome",
            "last_name": "NovoSobrenome",
            "email": "novoemail@example.com",
            "cell_phone": "NovoTelefone"
        }
    } } }
)
```


Remover uma tarefa de um projeto específico:
```
db.Project.updateOne(
    { _id: ObjectId("ID_do_Projeto_Aqui") },
    { $pull: { "tasks": { "title": "TarefaParaRemover" } } }
)
```


Atualizar o nome e a data de início de um projeto específico:
```
db.Project.updateOne(
    { _id: ObjectId("ID_do_Projeto_Aqui") },
    { $set: { "name": "Novo Nome do Projeto", "start_date": ISODate("NovaDataDeInicioAqui") } }
)
```
