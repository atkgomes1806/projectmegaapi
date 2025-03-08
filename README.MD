<h1 align="center">
  <br />
  <img
    src="./_docs/assets/icon.png"
    alt="Mega Man Robots API"
    width="150"
  />
  <br />
  <b>Mega Man Robots API</b>
  <br />
  <sub><sup><b>(MEGA-MAN-ROBOTS)</b></sup></sub>
  <br />
  <a href="https://github.com/felipeAguiarCode/MegaApiDotnetCore/actions/workflows/build.yml">
    <img
      src="https://github.com/felipeAguiarCode/MegaApiDotnetCore/actions/workflows/build.yml/badge.svg"
      alt="Build Status"
    />
  </a>
  <a href="https://github.com/felipeAguiarCode/MegaApiDotnetCore/releases/latest">
    <img
      src="https://img.shields.io/github/v/release/felipeAguiarCode/MegaApiDotnetCore"
      alt="Latest Release"
    />
  </a>
</h1>

<p align="center">
  API desenvolvida com .NET Core 3.1 para fornecer dados em JSON sobre os chefes da série Mega Man.
  <br />
</p>

<p align="center">
  Desenvolvido com <b>Entity Framework Core</b> e outras tecnologias modernas do .NET, este projeto visa fornecer uma API robusta para acessar dados dos robôs de Mega Man.
</p>

<p align="center">
  <br />
  <img src="./_docs/assets/carbon.png" alt="Code Preview"/>
</p>

## 📌 API Endpoints

<table align="center">
  <tr>
    <th>Método</th>
    <th>Endpoint</th>
    <th>Descrição</th>
  </tr>
  <tr>
    <td>GET</td>
    <td>/api/v1/robots</td>
    <td>Retorna uma lista de todos os robôs</td>
  </tr>
  <tr>
    <td>GET</td>
    <td>/api/v1/robots/{id}</td>
    <td>Retorna detalhes de um robô específico pelo ID</td>
  </tr>
  <tr>
    <td>POST</td>
    <td>/api/v1/robots</td>
    <td>Cria uma nova entrada de robô</td>
  </tr>
</table>

### 🔹 Exemplo de Resposta JSON

```json
{
  "id": 1,
  "name": "Metal Man",
  "game": "Mega Man 2",
  "weakness": "Quick Boomerang"
}
```

## ⚙️ Tecnologias Utilizadas

- **[Entity Framework Core](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8)** - ORM para gerenciamento de dados.
- **[RESTful API Design](https://restfulapi.net/) ** - Padrão para comunicação eficiente.
- **[Dependency Injection](https://learn.microsoft.com/en-us/dotnet/core/extensions/dependency-injection)** - Promove baixo acoplamento e melhor testabilidade.

## 📦 Dependências

| Pacote | Versão | Link |
|--------|--------|------|
| **[Microsoft.EntityFrameworkCore](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8)** | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/3.1.8) |
| **[Microsoft.EntityFrameworkCore.Design](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8)** | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/3.1.8) |
| **[Microsoft.EntityFrameworkCore.SqlServer](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8)** | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/3.1.8) |
| **[Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json/12.0.2)** | 12.0.2 | [NuGet](https://www.nuget.org/packages/Newtonsoft.Json/12.0.2) |

## 🏗️ Estrutura do Projeto

```🌐
src
├── 📂 Controllers      [Rotas para os endpoints]
├── 📂 Models           [Modelos do banco de dados]
├── 📂 Services         [Regras de negócio]
├── 📂 Middlewares      [Funções intermediárias para requisições HTTP]
├── 📂 Database         [Estruturas do banco de dados]
│   ├── 📂 DTOs             [Modelos de entrada e saída]
│   ├── 📂 EntityFramework  [Arquivos do Entity Framework]
│   │     ├── 📂 Context         [Configurações do contexto do banco]
│   │     ├── 📂 Migrations      [Migrações do banco de dados]
│   ├── 📂 Repositories     [Padrão de repositório]
```

## 🚀 Planejamento Futuro

- Atualizar para .NET 6.
- Implementar autenticação via JWT.
- Melhorar a documentação com OpenAPI (Swagger).
- Adicionar mais detalhes sobre cada robô (habilidades, fraquezas, etc.).

## 📜 Licença
Este software está licenciado sob os termos da [MIT License](https://opensource.org/licenses/MIT).

👨‍💻 Desenvolvido por **Felipe Aguiar** - [GitHub](https://github.com/felipeAguiarCode)

