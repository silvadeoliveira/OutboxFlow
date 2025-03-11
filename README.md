# OutboxFlow - Padrão Outbox em Microsserviços Bancários

## 📌 Sobre o Projeto
O **OutboxFlow** é um projeto desenvolvido para demonstrar a implementação do **Padrão Outbox** em **ASP.NET Core 8**, garantindo entrega confiável de eventos em um ambiente de microsserviços bancários.

Este projeto visa resolver problemas comuns em sistemas distribuídos, como perda de mensagens, inconsistências de dados e falhas na comunicação entre serviços.

## 📖 Contexto e Inspiração
Este repositório foi inspirado pelo artigo de **David Shergilashvili** sobre o **Outbox Pattern em Microsserviços Bancários**. Mais detalhes podem ser encontrados no post original:
🔗 [Outbox Pattern in Banking Microservices - David Shergilashvili](https://www.linkedin.com/pulse/outbox-pattern-banking-microservices-david-shergilashvili-mlg1f/)

Além disso, compartilhei minha visão sobre o tema no meu post no LinkedIn: 
🔗 [Meu post sobre Outbox Pattern](#) *(Substitua pelo link do seu post no LinkedIn)*

## 🚀 Tecnologias Utilizadas
- **ASP.NET Core 8**
- **Entity Framework Core** (EF Core)
- **PostgreSQL**
- **RabbitMQ**
- **Docker** (para ambientes de testes)
- **Background Services** para processamento assíncrono

## 🔥 Funcionalidades Implementadas
✅ Gravação de eventos na tabela **Outbox** dentro da mesma transação do banco de dados.
✅ Processador de Outbox que lê eventos pendentes e os publica no **RabbitMQ**.
✅ Garantia de **entrega confiável** e **resiliência** contra falhas do sistema.
✅ Exemplo de **consumidor RabbitMQ** para processar os eventos recebidos.

## 🛠️ Como Executar o Projeto
### 📌 Pré-requisitos
- .NET 8 SDK instalado
- Docker instalado (para o RabbitMQ e banco de dados)

### 📌 Passos para rodar o projeto
1️⃣ Clone este repositório:
```bash
git clone https://github.com/silvadeoliveira/OutboxFlow
cd outboxflow
```
2️⃣ Configure o banco de dados e o RabbitMQ via Docker:
```bash
docker-compose up -d
```
3️⃣ Execute a aplicação:
```bash
dotnet run
```

## 🤝 Contribuições
Sinta-se à vontade para abrir issues e pull requests caso tenha sugestões de melhorias!

---
**Criado por [Fabio Oliveira]** – Conecte-se comigo no [LinkedIn](#) *(https://www.linkedin.com/in/fabio-oliveira-4447b021/)* 🚀
