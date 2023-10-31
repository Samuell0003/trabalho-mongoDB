```
db.Project.createIndex({ "tasks.status": 1 })
```
```
db.Project.createIndex({ "start_date": 1, "end_date": 1 })
```


Infelizmente nao consegui encontrar diferença de desempenho com os índices criados, por conta da pouca quantidade de dados.
