# Mega Man Robots API

<p align="center">
  <img src="./_docs/assets/icon.png" alt="Mega Man Robots API" width="150" />
</p>

<p align="center">
  <b>Uma API RESTful para acessar dados dos chefes da série Mega Man</b>
</p>

<p align="center">
  <a href="https://github.com/felipeAguiarCode/MegaApiDotnetCore/actions/workflows/build.yml">
    <img src="https://github.com/felipeAguiarCode/MegaApiDotnetCore/actions/workflows/build.yml/badge.svg" alt="Build Status" />
  </a>
  <a href="https://github.com/felipeAguiarCode/MegaApiDotnetCore/releases/latest">
    <img src="https://img.shields.io/github/v/release/felipeAguiarCode/MegaApiDotnetCore" alt="Latest Release" />
  </a>
</p>

## 📘 Descrição

A **Mega Man Robots API** é um serviço backend desenvolvido em **.NET Core 3.1** para fornecer dados sobre os chefes da franquia Mega Man. A API retorna informações em **formato JSON** e pode ser utilizada em aplicações que precisem consultar detalhes sobre os robôs da série.

> **🚀 Planejamento Futuro**: Atualizar para **.NET 6+** para melhorar a performance e segurança.

## 📌 Endpoints da API

| Método | Endpoint              | Descrição                                      |
|--------|-----------------------|------------------------------------------------|
| `GET`  | `/api/v1/robots`      | Retorna a lista completa de robôs            |
| `GET`  | `/api/v1/robots/{id}` | Retorna detalhes de um robô específico        |
| `POST` | `/api/v1/robots`      | Cria um novo robô                             |

### 📡 Exemplo de Resposta

```json
{
  "id": 1,
  "name": "Cut Man",
  "game": "Mega Man (1987)",
  "weakness": "Super Arm",
  "description": "Cut Man foi projetado para cortar árvores, mas acabou se tornando um inimigo formidável."
}
```

## ⚙️ Tecnologias Utilizadas

- **.NET Core 3.1** → (Planejada migração para .NET 6+)
- **Entity Framework Core** → ORM para gerenciamento de dados
- **RESTful API Design** → Arquitetura baseada em boas práticas REST
- **Dependency Injection** → Promove desacoplamento e testabilidade

## 📦 Dependências Principais

| Pacote                                  | Versão  |
|-----------------------------------------|---------|
| `Microsoft.EntityFrameworkCore`        | 3.1.8   |
| `Microsoft.EntityFrameworkCore.Design` | 3.1.8   |
| `Microsoft.EntityFrameworkCore.SqlServer` | 3.1.8 |
| `Newtonsoft.Json`                       | 12.0.2  |

## 🏗 Arquitetura do Projeto

```
📂 src
├── 📂 Controllers      [Gerencia os endpoints]
├── 📂 Models           [Definição dos modelos de dados]
├── 📂 Services         [Regras de negócio e lógica da aplicação]
├── 📂 Middlewares      [Interceptação e manipulação de requisições]
├── 📂 Database         [Estruturas relacionadas ao banco de dados]
│   ├── 📂 DTOs        [Data Transfer Objects]
│   ├── 📂 EntityFramework  [Contexto e Migrations]
│   │     ├── 📂 Context         [Configuração do contexto do EF]
│   │     ├── 📂 Migrations      [Histórico de alterações no banco]
│   ├── 📂 Repositories  [Padrão Repository para acesso aos dados]
```

## 📜 Licença

Este projeto é licenciado sob os termos da licença **MIT**. Para mais detalhes, consulte o arquivo [`LICENSE`](LICENSE).

## 🙋‍♂️ Autor

Criado por **Felipe Aguiar**.
- 📌 GitHub: [felipeAguiarCode](https://github.com/felipeAguiarCode)
