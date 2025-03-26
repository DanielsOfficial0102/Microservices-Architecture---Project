# 🛍️ Plataforma de E-commerce para Startup de Vestuário  

Este repositório contém a arquitetura de microsserviços desenvolvida para uma **plataforma de e-commerce** baseada no conceito de **Guide Shop**. O projeto foi criado como parte de um estudo acadêmico, aplicando boas práticas de arquitetura distribuída e escalável.  

## 📌 Sobre o Projeto  
A proposta é desenvolver uma solução para um **Guide Shop**, onde os clientes podem:  
✔️ **Comprar na loja física** usando um tablet com auxílio de um vendedor ou um totem de autoatendimento.  
✔️ **Receber o pedido no mesmo dia** via centros de distribuição locais.  
✔️ **Acompanhar a entrega em tempo real** pelo aplicativo.  

## 🏗️ Arquitetura  

A solução foi projetada utilizando **microsserviços**, garantindo escalabilidade, resiliência e alta disponibilidade.  

### 🔹 **Diagrama da Arquitetura**  
![Diagrama da Arquitetura](microservices_architecture_fixed.drawio.png)  

### 📖 **Legenda das Etapas**  

1️⃣ **Canais de Entrada**: Website, App Mobile, Tablets, Totens.  
2️⃣ **API Gateway**: Ponto único de entrada para roteamento e segurança.  
3️⃣ **BFF Mobile/Web**: Backend otimizado para cada plataforma.  
4️⃣ **Load Balancer**: Distribuição de carga entre os microsserviços.  
5️⃣ **Order Service**: Processamento de pedidos.  
6️⃣ **Payment Gateway (Pagar.me)**: Processamento de pagamentos.  
7️⃣ **User Service**: Autenticação e gerenciamento de perfis.  
8️⃣ **Product Catalog (Redis Cache)**: Catálogo de produtos otimizado.  
9️⃣ **Inventory Service**: Controle de estoque.  
🔟 **Databases (PostgreSQL/MongoDB)**: Armazenamento de dados.  
1️⃣1️⃣ **Observability Stack (Prometheus, Grafana, ELK)**: Monitoramento e logs.  
1️⃣2️⃣ **Redis (Caching)**: Cache para alta performance.  
1️⃣3️⃣ **Shipping & Tracking**: Gestão de entregas e rastreamento.  
1️⃣4️⃣ **Local Fulfillment Center**: Centros de distribuição regionais.  
1️⃣5️⃣ **User Monitoring**: Acompanhamento do usuário.  
1️⃣6️⃣ **Load Balancer Adicional**: Balanceamento interno.  
1️⃣7️⃣ **Message Broker (Kafka/RabbitMQ)**: Comunicação assíncrona.  
1️⃣8️⃣ **Notification Service**: Envio de notificações via e-mail, SMS e push.  

---

## 🚀 Tecnologias Utilizadas  

- **API Gateway** para gerenciamento de tráfego  
- **BFF (Backend for Frontend)** para otimização de comunicação  
- **Load Balancer** para distribuir requisições  
- **Redis Cache** para melhorar a performance do catálogo de produtos  
- **RabbitMQ/Kafka** para comunicação assíncrona entre microsserviços  
- **PostgreSQL & MongoDB** para armazenamento de dados  
- **Prometheus, Grafana, ELK** para observabilidade e logs  

## 👥 Grupo
### Bruno Elly
### Bruno Lima
### Daniel Lopes
### Gabriel Anchieta

## 📌 Como Utilizar  

1️⃣ Clone este repositório:  
```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
