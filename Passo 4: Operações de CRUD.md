#"Crie 15 queries para busca de projetos, tarefas e usuários";

##"Buscar todos os projetos com data de início após uma data específica (por exemplo, 2023-01-01)":
db.Project.find({ start_date: { $gte: ISODate("2023-01-01") } })


##"Buscar todas as tarefas com status "Em andamento" de um projeto específico":
db.Task.find({ project_id: ObjectId("project_id_here"), status: "Em andamento" })


##Buscar todos os usuários cujo primeiro nome comece com "John":
db.User.find({ first_name: /^John/i })


##Buscar todas as tarefas com prioridade "Alta" ou "Média" de um projeto específico:
db.Task.find({ project_id: ObjectId("project_id_here"), priority: { $in: ["Alta", "Média"] } })


##Buscar todos os projetos com nome que contenha uma palavra-chave (por exemplo, "projeto") e data de término no futuro:
db.Project.find({ name: { $regex: /projeto/i }, end_date: { $gte: new Date() } })


##Buscar todas as tarefas atribuídas a usuários com um determinado domínio de e-mail (por exemplo, "@example.com"):
db.Task.find({ "user.email": { $regex: /@example.com$/i } })


##Buscar todos os projetos ordenados por data de término em ordem crescente:
db.Project.find({}).sort({ end_date: 1 })


##Buscar todas as tarefas com uma descrição que contenha uma palavra específica (por exemplo, "importante"):
db.Task.find({ description: { $regex: /importante/i } })


##Buscar todos os usuários que não têm um número de telefone celular especificado:
db.User.find({ cell_phone: { $exists: false } })


##Buscar todos os projetos com data de término no mês atual:
db.Project.find({
    end_date: {
        $gte: new Date(new Date().getFullYear(), new Date().getMonth(), 1),
        $lt: new Date(new Date().getFullYear(), new Date().getMonth() + 1, 1)
    }
})
