Modelagem banco de dados
```
db.createCollection("Project", {
    validator: {
        $jsonSchema: {
            bsonType: "object",
            required: ["name", "start_date", "end_date", "tasks"],
            properties: {
                name: {
                    bsonType: "string",
                    description: "Deve ser uma string representando o nome do projeto."
                },
                start_date: {
                    bsonType: "date",
                    description: "Deve ser uma data representando a data de início do projeto."
                },
                end_date: {
                    bsonType: "date",
                    description: "Deve ser uma data representando a data de término do projeto."
                },
                tasks: {
                    bsonType: "array",
                    description: "Deve ser uma lista representando as tasks",
                    items: {
                        bsonType: "object",
                        required: ["title", "description", "start_date", "deadline_date", "priority", "status", "user"],

                        properties: {
                            title: {
                                bsonType: "string",
                                description: "Deve ser uma string representando o título da tarefa."
                            },
                            description: {
                                bsonType: "string",
                                description: "Deve ser uma string representando a descrição da tarefa."
                            },
                            start_date: {
                                bsonType: "date",
                                description: "Deve ser uma data representando a data de início da tarefa."
                            },
                            deadline_date: {
                                bsonType: "date",
                                description: "Deve ser uma data representando a data limite da tarefa."
                            },
                            priority: {
                                bsonType: "string",
                                description: "Deve ser uma string representando a prioridade da tarefa."
                            },
                            status: {
                                bsonType: "string",
                                description: "Deve ser uma string representando o status da tarefa."
                            },
                            user: {
                                bsonType: "object",
                                description: "Deve ser um object representando o usuario",
                                required: ["first_name", "last_name", "email", "cell_phone"],
                                properties: {
                                    first_name: {
                                        bsonType: "string",
                                        description: "Deve ser uma string representando o primeiro nome do usuário."
                                    },
                                    last_name: {
                                        bsonType: "string",
                                        description: "Deve ser uma string representando o sobrenome do usuário."
                                    },
                                    email: {
                                        bsonType: "string",
                                        description: "Deve ser uma string representando o endereço de e-mail do usuário.",
                                        pattern: "^\\S+@\\S+\\.\\S+$" // Expressão regular para validar o formato do e-mail.
                                    },
                                    cell_phone: {
                                        bsonType: "string",
                                        description: "Deve ser uma string representando o número de telefone celular do usuário."
                                    }
                                }
                            }


                        }
                    }
                }
            }
        }
    }
})
```

Exemplo JSON
```
{
    "name": "Projeto A",
    "start_date": "2023-01-01",
    "end_date": "2023-12-31",
    "tasks": [
        {
            "title": "Tarefa 1",
            "description": "Descrição da Tarefa 1",
            "start_date": "2023-01-15",
            "deadline_date": "2023-02-15",
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
            "start_date": "2023-02-01",
            "deadline_date": "2023-03-01",
            "priority": "Média",
            "status": "Concluída",
            "user": {
                "first_name": "Jane",
                "last_name": "Smith",
                "email": "janesmith@example.com",
                "cell_phone": "987-654-3210"
            }
        },
        ...
    ]
}
```
