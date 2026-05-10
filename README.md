# 📍 Busca CEP - Sistema Integrado de Gerenciamento de Endereços

Um sistema web *Full-Stack* desenvolvido para buscar, cadastrar e gerenciar endereços de forma personalizada, utilizando a API pública do ViaCEP. O projeto conta com autenticação de usuários e isolamento de dados, garantindo que cada usuário acesse apenas os seus próprios endereços salvos.

## 🚀 Funcionalidades

- **Cadastro e Autenticação:** Criação de conta e login de usuários.
- **Integração de API Externa:** Consulta de endereços em tempo real via [ViaCEP](https://viacep.com.br/).
- **Gerenciamento de Endereços:** Salva os resultados da busca diretamente no banco de dados.
- **Isolamento de Dados:** Cada usuário visualiza e gerencia exclusivamente sua própria lista de endereços.
- **Exclusão:** Permite ao usuário deletar endereços previamente salvos.

## 🛠️ Tecnologias e Padrões Utilizados

**Back-end:**
- C# / ASP.NET Core Web API
- Entity Framework Core (ORM)
- MySQL (Banco de Dados Relacional)
- **Conceitos Aplicados:** Arquitetura RESTful, Padrão MVC (Models/Controllers), Injeção de Dependência, DTOs (*Data Transfer Objects*) para segurança de tráfego de dados e *JsonIgnore* para proteção de dados sensíveis.

**Front-end:**
- HTML5 & CSS3
- JavaScript Vanilla (Consumo de API via `Fetch`)

## 📋 Pré-requisitos

Para rodar este projeto na sua máquina, você precisará ter instalado:
- [.NET SDK](https://dotnet.microsoft.com/download)
- Servidor MySQL rodando localmente na porta padrão.
- Editor de código (recomendado: [Visual Studio Code](https://code.visualstudio.com/)).
- Extensão **Live Server** instalada no VS Code para rodar o Front-end.

## ⚙️ Como Rodar o Projeto

**1. Configurando o Banco de Dados:**
Abra o terminal na pasta raiz do projeto (onde está o arquivo `.csproj`) e execute as *migrations* para criar o banco de dados e as tabelas:
```bash
dotnet ef database update
2. Iniciando o Servidor Back-end:
Ainda no terminal, inicie a aplicação ASP.NET:

Bash
dotnet run
O servidor estará rodando, geralmente, em http://localhost:5000 ou na porta configurada no seu launchSettings.json.

3. Iniciando o Cliente (Front-end):

Abra a pasta do Front-end no VS Code.

Clique com o botão direito no arquivo index.html e selecione "Open with Live Server".

O projeto abrirá no seu navegador, pronto para uso!

👨‍💻 Autor
Davi Oliveira Silva

LinkedIn: www.linkedin.com/in/davi-oliveira-48b8501a3    

GitHub: https://github.com/Nivel999/Busca-CEP

E-mail: davioliveira1737@gmail.com