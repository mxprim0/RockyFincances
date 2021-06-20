# RockyFincances | [![Codacy Badge](https://app.codacy.com/project/badge/Grade/3526f61815d14ba480c68d90cc075ff4)](https://www.codacy.com/gh/dan-primo/RockyFincances/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=dan-primo/RockyFincances&amp;utm_campaign=Badge_Grade)
CRUD utilizando ASP.NET Core MVC .NET 5, Entity Framework e SQL Server

### Desafio Técnico para Backend

### [Resumo do Projeto Rocky Finances, aqui eu conto como é o projeto, meus desafios e aprendizados além é claro, dos próximos passos.](https://www.notion.so/Rocky-Finances-3138984f306540b583465269f69b7fe1)

### Para rodar localmente é necessário ter o Visual Studio ou VSCode e SQL Server.

1. Faça o clone ou dowload desse projeto localmente:

``
git clone https://github.com/dan-primo/RockyFincances.git
``

2. Abra o arquivo de solução do projeto chamado Rocky.sln

3. Recompile a Solução do projeto, pode ser pelo atalho Ctrl + Alt + F7

4. Faça a conexão com algum banco de dados local, alterando o endereço da "DefaultConnection" para sua conexão local no arquivo appsettings.json:
``
{
  "ConnectionStrings": {
    "DefaultConnection": "Server= Insira aqui o nome do enderço do seu servidor local;Database=Rocky;Trusted_Connection=True;MultipleActiveResultSets=True"
  },
  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft": "Warning",
      "Microsoft.Hosting.Lifetime": "Information"
    }
  },
  "AllowedHosts": "*"
}
``

5. Restaure os pacotes NuGet da Solução:
Pelo CLI: 
``
dotnet restore
``
Pelo CLI do Nuget: 
``
nuget restore Rocky.sln
``

6. Execute as migrations do projeto para restaurar as tabelas do banco de dados:
Abra o Console do Gerenciador de Pacotes e rode o comando:
``
update-database
``
Para verificar se deu certo você pode abrir o SQL Server Object Explorer e verificar se o banco de dados "Rocky" consta na lista de Databases local.

7. Por fim, recompile a solução: Crtl + Alt + F7 e em seguida execute a solução Rocky.sln 

### Tecnologias utilizadas:

* Dotnet 5.0
* SQL Server
* EntityFrameworkCore
* SwaggerUI (branch swagger, em construção)
