# 📍 Busca CEP - Sistema Integrado de Gerenciamento de Endereços

Um sistema web *Full-Stack* desenvolvido para buscar, cadastrar e gerenciar endereços de forma personalizada, utilizando a API pública do ViaCEP. O projeto conta com autenticação de usuários e isolamento de dados, garantindo que cada usuário acesse apenas os seus próprios endereços salvos.

---

## 🚀 Funcionalidades

- **Cadastro e Autenticação:** Criação de conta e login de usuários.
- **Integração de API Externa:** Consulta de endereços em tempo real via [ViaCEP](https://viacep.com.br/).
- **Gerenciamento de Endereços:** Salva os resultados da busca diretamente no banco de dados.
- **Isolamento de Dados:** Cada usuário visualiza e gerencia exclusivamente sua própria lista de endereços.
- **Exclusão:** Permite ao usuário deletar endereços previamente salvos.

---

## 🛠️ Tecnologias e Padrões Utilizados

### **Back-end**
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Entity Framework](https://img.shields.io/badge/EF%20Core-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)

- **Conceitos Aplicados:** Arquitetura RESTful, Padrão MVC (Models/Controllers), Injeção de Dependência, DTOs (*Data Transfer Objects*) para segurança de tráfego de dados e *JsonIgnore* para proteção de dados sensíveis.

### **Front-end**
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black)

- **Consumo de API:** Interface responsiva consumindo dados via `Fetch API`.

---

## 📋 Pré-requisitos

Para rodar este projeto na sua máquina, você precisará ter instalado:
- [.NET SDK](https://dotnet.microsoft.com/download)
- Servidor MySQL rodando localmente.
- Editor de código (recomendado: [Visual Studio Code](https://code.visualstudio.com/)).
- Extensão **Live Server** instalada no VS Code para o Front-end.

---

## ⚙️ Como Rodar o Projeto

### **1. Configurando o Banco de Dados**
Antes de iniciar, configure a sua *Connection String* no arquivo `appsettings.json` localizado dentro da pasta `Server`, inserindo o seu usuário e senha do MySQL.

Após configurar, abra o terminal na raiz do projeto e execute:
```bash
cd Server
dotnet ef database update
2. Iniciando o Servidor (Back-end)
Ainda no terminal, dentro da pasta Server, execute o comando:

Bash
dotnet run
O servidor estará disponível em http://localhost:5000 (ou na porta configurada no seu ambiente).

3. Iniciando o Cliente (Front-end)
No VS Code, abra a pasta Client.

Clique com o botão direito no arquivo index.html.

Selecione "Open with Live Server".

O sistema abrirá automaticamente no seu navegador.

👨‍💻 Autor
Davi Oliveira Silva
