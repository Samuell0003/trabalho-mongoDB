insercao de dados
```
db.Project.insertOne(
    {
        "name": "Projeto A",
        "start_date": ISODate("2023-01-01"),
        "end_date": ISODate("2023-12-31"),
        "tasks": [
            {
                "title": "Tarefa 1",
                "description": "Descrição da Tarefa 1",
                "start_date": ISODate("2023-01-15"),
                "deadline_date": ISODate("2023-02-15"),
                "priority": "Alta",
                "status": "Em andamento",
                "user": {
                    "first_name": "John",
                    "last_name": "Doe",
                    "email": "johndoe@example.com",
                    "cell_phone": "123-456-7890"
                }
            },
            {
                "title": "Tarefa 2",
                "description": "Descrição da Tarefa 2",
                "start_date": ISODate("2023-02-01"),
                "deadline_date": ISODate("2023-03-01"),
                "priority": "Média",
                "status": "Concluída",
                "user": {
                    "first_name": "Jane",
                    "last_name": "Smith",
                    "email": "janesmith@example.com",
                    "cell_phone": "987-654-3210"
                }
            },
            {
                "title": "Tarefa 3",
                "description": "Descrição da Tarefa 3",
                "start_date": ISODate("2023-04-15"),
                "deadline_date": ISODate("2023-05-15"),
                "priority": "Baixa",
                "status": "Pendente",
                "user": {
                    "first_name": "Alice",
                    "last_name": "Johnson",
                    "email": "alice@example.com",
                    "cell_phone": "555-555-1234"
                }
            },
            {
                "title": "Tarefa 4",
                "description": "Descrição da Tarefa 4",
                "start_date": ISODate("2023-06-01"),
                "deadline_date": ISODate("2023-07-01"),
                "priority": "Alta",
                "status": "Em andamento",
                "user": {
                    "first_name": "Bob",
                    "last_name": "Williams",
                    "email": "bob@example.com",
                    "cell_phone": "555-555-5678"
                }
            },
            {
                "title": "Tarefa 5",
                "description": "Descrição da Tarefa 5",
                "start_date": ISODate("2023-08-15"),
                "deadline_date": ISODate("2023-09-15"),
                "priority": "Média",
                "status": "Pendente",
                "user": {
                    "first_name": "Eva",
                    "last_name": "Brown",
                    "email": "eva@example.com",
                    "cell_phone": "555-555-9090"
                }
            },
            {
                "title": "Tarefa 5",
                "description": "Descrição da Tarefa 5",
                "start_date": ISODate("2023-08-15"),
                "deadline_date": ISODate("2023-09-15"),
                "priority": "Média",
                "status": "Pendente",
                "user": {
                    "first_name": "Eva",
                    "last_name": "Brown",
                    "email": "eva@example.com",
                    "cell_phone": "555-555-9090"
                }
            },
            {
                "title": "Tarefa 6",
                "description": "Descrição da Tarefa 6",
                "start_date": ISODate("2023-10-01"),
                "deadline_date": ISODate("2023-11-01"),
                "priority": "Alta",
                "status": "Em andamento",
                "user": {
                    "first_name": "David",
                    "last_name": "Jones",
                    "email": "david@example.com",
                    "cell_phone": "555-555-1212"
                }
            },
            {
                "title": "Tarefa 7",
                "description": "Descrição da Tarefa 7",
                "start_date": ISODate("2023-11-15"),
                "deadline_date": ISODate("2023-12-15"),
                "priority": "Baixa",
                "status": "Pendente",
                "user": {
                    "first_name": "Grace",
                    "last_name": "Davis",
                    "email": "grace@example.com",
                    "cell_phone": "555-555-3434"
                }
            },
            {
                "title": "Tarefa 8",
                "description": "Descrição da Tarefa 8",
                "start_date": ISODate("2023-12-01"),
                "deadline_date": ISODate("2024-01-01"),
                "priority": "Média",
                "status": "Concluída",
                "user": {
                    "first_name": "Peter",
                    "last_name": "Moore",
                    "email": "peter@example.com",
                    "cell_phone": "555-555-5656"
                }
            },
            {
                "title": "Tarefa 9",
                "description": "Descrição da Tarefa 9",
                "start_date": ISODate("2024-01-15"),
                "deadline_date": ISODate("2024-02-15"),
                "priority": "Alta",
                "status": "Pendente",
                "user": {
                    "first_name": "Linda",
                    "last_name": "Wilson",
                    "email": "linda@example.com",
                    "cell_phone": "555-555-7878"
                }
            },
            {
                "title": "Tarefa 10",
                "description": "Descrição da Tarefa 10",
                "start_date": ISODate("2024-02-29"),
                "deadline_date": ISODate("2024-03-30"),
                "priority": "Média",
                "status": "Em andamento",
                "user": {
                    "first_name": "Michael",
                    "last_name": "Taylor",
                    "email": "michael@example.com",
                    "cell_phone": "555-555-9090"
                }
            },
            {
                "title": "Tarefa 11",
                "description": "Descrição da Tarefa 11",
                "start_date": ISODate("2024-04-15"),
                "deadline_date": ISODate("2024-05-15"),
                "priority": "Alta",
                "status": "Em andamento",
                "user": {
                    "first_name": "Sarah",
                    "last_name": "Wilson",
                    "email": "sarah@example.com",
                    "cell_phone": "555-555-9898"
                }
            },
            {
                "title": "Tarefa 12",
                "description": "Descrição da Tarefa 12",
                "start_date": ISODate("2024-05-30"),
                "deadline_date": ISODate("2024-06-30"),
                "priority": "Média",
                "status": "Concluída",
                "user": {
                    "first_name": "George",
                    "last_name": "Anderson",
                    "email": "george@example.com",
                    "cell_phone": "555-555-1212"
                }
            },
            {
                "title": "Tarefa 13",
                "description": "Descrição da Tarefa 13",
                "start_date": ISODate("2024-07-15"),
                "deadline_date": ISODate("2024-08-15"),
                "priority": "Baixa",
                "status": "Pendente",
                "user": {
                    "first_name": "Mia",
                    "last_name": "Roberts",
                    "email": "mia@example.com",
                    "cell_phone": "555-555-3434"
                }
            },
            {
                "title": "Tarefa 14",
                "description": "Descrição da Tarefa 14",
                "start_date": ISODate("2024-09-01"),
                "deadline_date": ISODate("2024-10-01"),
                "priority": "Alta",
                "status": "Em andamento",
                "user": {
                    "first_name": "John",
                    "last_name": "Smith",
                    "email": "john@example.com",
                    "cell_phone": "555-555-5656"
                }
            },
            {
                "title": "Tarefa 15",
                "description": "Descrição da Tarefa 15",
                "start_date": ISODate("2024-10-15"),
                "deadline_date": ISODate("2024-11-15"),
                "priority": "Média",
                "status": "Pendente",
                "user": {
                    "first_name": "Emily",
                    "last_name": "Brown",
                    "email": "emily@example.com",
                    "cell_phone": "555-555-7878"
                }
            },
            {
                "title": "Tarefa 16",
                "description": "Descrição da Tarefa 16",
                "start_date": ISODate("2024-10-20"),
                "deadline_date": ISODate("2024-11-20"),
                "priority": "Alta",
                "status": "Em andamento",
                "user": {
                    "first_name": "John",
                    "last_name": "Smith",
                    "email": "john@example.com",
                    "cell_phone": "123-456-7890"
                }
            },
            {
                "title": "Tarefa 17",
                "description": "Descrição da Tarefa 17",
                "start_date": ISODate("2024-10-25"),
                "deadline_date": ISODate("2024-11-25"),
                "priority": "Baixa",
                "status": "Concluída",
                "user": {
                    "first_name": "Alice",
                    "last_name": "Johnson",
                    "email": "alice@example.com",
                    "cell_phone": "987-654-3210"
                }
            },
            {
                "title": "Tarefa 18",
                "description": "Descrição da Tarefa 18",
                "start_date": ISODate("2024-10-30"),
                "deadline_date": ISODate("2024-11-30"),
                "priority": "Média",
                "status": "Pendente",
                "user": {
                    "first_name": "David",
                    "last_name": "Davis",
                    "email": "david@example.com",
                    "cell_phone": "111-222-3333"
                }
            },
            {
                "title": "Tarefa 19",
                "description": "Descrição da Tarefa 19",
                "start_date": ISODate("2024-11-05"),
                "deadline_date": ISODate("2024-12-05"),
                "priority": "Alta",
                "status": "Em andamento",
                "user": {
                    "first_name": "Sophia",
                    "last_name": "Martinez",
                    "email": "sophia@example.com",
                    "cell_phone": "555-123-4567"
                }
            },
            {
                "title": "Tarefa 20",
                "description": "Descrição da Tarefa 20",
                "start_date": ISODate("2024-11-10"),
                "deadline_date": ISODate("2024-12-10"),
                "priority": "Baixa",
                "status": "Pendente",
                "user": {
                    "first_name": "Michael",
                    "last_name": "Anderson",
                    "email": "michael@example.com",
                    "cell_phone": "555-777-8888"
                }
            },
            {
                "title": "Tarefa 21",
                "description": "Descrição da Tarefa 21",
                "start_date": ISODate("2024-11-15"),
                "deadline_date": ISODate("2024-12-15"),
                "priority": "Média",
                "status": "Em andamento",
                "user": {
                    "first_name": "Linda",
                    "last_name": "Wilson",
                    "email": "linda@example.com",
                    "cell_phone": "111-333-5555"
                }
            },
            {
                "title": "Tarefa 22",
                "description": "Descrição da Tarefa 22",
                "start_date": ISODate("2024-11-20"),
                "deadline_date": ISODate("2024-12-20"),
                "priority": "Alta",
                "status": "Concluída",
                "user": {
                    "first_name": "Daniel",
                    "last_name": "Thomas",
                    "email": "daniel@example.com",
                    "cell_phone": "555-888-9999"
                }
            },
            {
                "title": "Tarefa 23",
                "description": "Descrição da Tarefa 23",
                "start_date": ISODate("2024-11-25"),
                "deadline_date": ISODate("2024-12-25"),
                "priority": "Média",
                "status": "Pendente",
                "user": {
                    "first_name": "Olivia",
                    "last_name": "Harris",
                    "email": "olivia@example.com",
                    "cell_phone": "777-222-1111"
                }
            },
            {
                "title": "Tarefa 24",
                "description": "Descrição da Tarefa 24",
                "start_date": ISODate("2024-11-30"),
                "deadline_date": ISODate("2024-12-30"),
                "priority": "Baixa",
                "status": "Em andamento",
                "user": {
                    "first_name": "James",
                    "last_name": "Clark",
                    "email": "james@example.com",
                    "cell_phone": "999-333-5555"
                }
            },
            {
                "title": "Tarefa 25",
                "description": "Descrição da Tarefa 25",
                "start_date": ISODate("2024-12-05"),
                "deadline_date": ISODate("2024-12-15"),
                "priority": "Alta",
                "status": "Em andamento",
                "user": {
                    "first_name": "Ava",
                    "last_name": "Moore",
                    "email": "ava@example.com",
                    "cell_phone": "555-666-7777"
                }
            },
            {
                "title": "Tarefa 26",
                "description": "Descrição da Tarefa 26",
                "start_date": ISODate("2024-12-10"),
                "deadline_date": ISODate("2024-12-20"),
                "priority": "Média",
                "status": "Concluída",
                "user": {
                    "first_name": "Liam",
                    "last_name": "Young",
                    "email": "liam@example.com",
                    "cell_phone": "777-888-9999"
                }
            },
            {
                "title": "Tarefa 27",
                "description": "Descrição da Tarefa 27",
                "start_date": ISODate("2024-12-15"),
                "deadline_date": ISODate("2024-12-25"),
                "priority": "Baixa",
                "status": "Pendente",
                "user": {
                    "first_name": "Mia",
                    "last_name": "Walker",
                    "email": "mia@example.com",
                    "cell_phone": "555-666-7777"
                }
            },
            {
                "title": "Tarefa 28",
                "description": "Descrição da Tarefa 28",
                "start_date": ISODate("2024-12-20"),
                "deadline_date": ISODate("2024-12-30"),
                "priority": "Alta",
                "status": "Em andamento",
                "user": {
                    "first_name": "Noah",
                    "last_name": "King",
                    "email": "noah@example.com",
                    "cell_phone": "555-888-9999"
                }
            },
            {
                "title": "Tarefa 29",
                "description": "Descrição da Tarefa 29",
                "start_date": ISODate("2024-12-25"),
                "deadline_date": ISODate("2025-01-05"),
                "priority": "Média",
                "status": "Pendente",
                "user": {
                    "first_name": "Emma",
                    "last_name": "Scott",
                    "email": "emma@example.com",
                    "cell_phone": "555-666-7777"
                }
            },
            {
                "title": "Tarefa 30",
                "description": "Descrição da Tarefa 30",
                "start_date": ISODate("2024-12-30"),
                "deadline_date": ISODate("2025-01-10"),
                "priority": "Baixa",
                "status": "Em andamento",
                "user": {
                    "first_name": "William",
                    "last_name": "Baker",
                    "email": "william@example.com",
                    "cell_phone": "555-888-9999"
                }
            }
        ]
    }
)
```
Result:
    {
      "acknowledged": true,
      "insertedId": {
        "$oid": "653fb03008f67cc3e3246fef"
      }
    }



#Crie 15 queries para busca de projetos, tarefas e usuários;

Buscar todos os projetos com data de início após uma data específica (por exemplo, 2023-01-01):
```
db.Project.find({ start_date: { $gte: ISODate("2023-01-01") } })
```

##Buscar todas as tarefas com status "Em andamento" de um projeto específico:
```
db.Project.aggregate([ { $unwind: "$tasks" }, { $match: { "tasks.status": "Em andamento"}}])
```

##Buscar todos os usuários cujo primeiro nome comece com "John":
```
db.Project.aggregate([ { $unwind: "$tasks" }, { $match: { "tasks.user.first_name": /^John/i}}])
```

##Buscar todas as tarefas com prioridade "Alta" ou "Média" de um projeto específico:
```
db.Project.aggregate([ { $unwind: "$tasks" }, { $match: { "tasks.priority": { $in: ["Alta", "Média"] }}}])
```


##Buscar todos os projetos com nome que contenha uma palavra-chave (por exemplo, "projeto") e data de término no futuro:
```
db.Project.find({ name: { $regex: /projeto/i }, end_date: { $gte: new Date() } })
```


##Buscar todas as tarefas atribuídas a usuários com um determinado domínio de e-mail (por exemplo, "@example.com"):
db.Task.find({ "user.email": { $regex: /@example.com$/i } })


##Buscar todos os projetos ordenados por data de término em ordem crescente:
```
db.Project.find({}).sort({ end_date: 1 })
```

##Buscar todas as tarefas com uma descrição que contenha uma palavra específica (por exemplo, "importante"):
db.Task.find({ description: { $regex: /importante/i } })


##Buscar todos os usuários que não têm um número de telefone celular especificado:
db.User.find({ cell_phone: { $exists: false } })


##Buscar todos os projetos com data de término no mês atual:
```
db.Project.find({
    end_date: {
        $gte: new Date(new Date().getFullYear(), new Date().getMonth(), 1),
        $lt: new Date(new Date().getFullYear(), new Date().getMonth() + 1, 1)
    }
})
```
