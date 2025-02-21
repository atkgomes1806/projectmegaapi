# MegaApiDotnetCore - Documentação

O projeto **MegaApiDotnetCore** é uma API desenvolvida em **.NET Core 3.1** para fornecer dados sobre chefes da série *Mega Man* em formato **JSON**. O projeto utiliza **Entity Framework Core** para gerenciamento de dados e segue um design **RESTful** para os endpoints da API.

## 📌 Descrição Geral
MegaApiDotnetCore é uma API backend que permite acessar informações sobre os robôs da franquia *Mega Man*. O projeto utiliza **dependência injeção**, **Entity Framework Core** e **padrão de repositório** para melhor organização e manutenção do código.

## 🔹 Técnicas usadas
- **Entity Framework Core:** ORM (Mapeamento Objeto-Relacional) para gerenciamento de dados.
- **RESTful API Design** - Garante pontos de comunicação claros e eficazes.
- **Dependency Injection** - Usada em todo o projeto para promover acoplamento fraco e maior testabilidade.

## 🔹 Principais Endpoints
| Método | Endpoint | Descrição |
|--------|------------|------------------------------------|
| GET    | `/api/v1/robots` | Retorna todos os robôs |
| GET    | `/api/v1/robots/{id}` | Retorna detalhes de um robô específico |
| POST   | `/api/v1/robots` | Cria um novo registro de robô |

## 🔹 Tecnologias Utilizadas
- **.NET Core 3.1** - Framework principal
- **Entity Framework Core** - ORM para acesso a banco de dados
- **Newtonsoft.Json** - Manipulação de JSON
- **SQL Server** - Banco de dados relacional

## 🔹 Dependências
| Pacote | Versão | Link |
|--------|------------|------------------------------------|
| Microsoft.EntityFrameworkCore    | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8) |
| Microsoft.EntityFrameworkCore.Design    | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8) |
| Microsoft.EntityFrameworkCore.SqlServer   | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8) |
| Newtonsoft.Json   | 12.0.2 | [NuGet](https://www.nuget.org/packages/Newtonsoft.Json/12.0.2) |

## 🔹 Estrutura do Projeto
```
src/
├── Controllers     # Rotas da API
├── Models          # Modelos de banco de dados
├── Services        # Regras de negócio
├── Middlewares     # Intermediários entre requisições e respostas
├── Database/
│   ├── DTOs              # Objetos de Transferência de Dados (Data Transfer Objects)
│   ├── EntityFramework/  # Configuração do ORM
│   │     ├── Context        # Configurações do contexto da entidade
│   │     ├── Migrations     # Migrações do banco de dados
│   ├── Repositories      # Implementação do padrão Repositório
```

## 🔹 Licença
O projeto é licenciado sob a **MIT License**, permitindo uso e modificação livre.

⌨️ Nelson -
[Github](https://github.com/santosnelson92)
