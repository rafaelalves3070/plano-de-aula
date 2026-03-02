# 🚀 Challenge Final – Projeto Integrador
O Challenge será iniciado a partir da Semana 8 e evoluirá até a Semana 12.

## 🎯 Tema
Sistema de Processamento de Pedidos Escalável

---
## 📦 Requisitos Técnicos

O projeto deverá integrar:

### 🔹 Arquitetura
- Separação em camadas
- Aplicação de SOLID
- Clean Code
- DTO + Mapper
- Tratamento global de exceções

### 🔹 Banco de Dados
- Modelagem relacional
- Normalização básica
- JPA/Hibernate
- Migrations (Flyway ou Liquibase)

### 🔹 Mensageria
- Evento: Pedido Criado
- Evento: Pedido Confirmado
- Publicação e consumo de eventos

Ferramenta sugerida:
- RabbitMQ ou Apache Kafka (conceito antes da ferramenta)

### 🔹 Testes
- Testes unitários em Service
- Testes de Controller
- Mocks adequados

### 🔹 Containerização
- Dockerfile
- docker-compose com:
    - API
    - Banco
    - Broker de mensageria

### 🔹 System Design
O aluno deverá ser capaz de explicar:

- Escalabilidade horizontal
- Separação de responsabilidades
- Motivo do uso de mensageria
- Estratégias de desacoplamento
- Como evoluir o sistema para alto volume

---
# 🏗️ Estrutura Esperada do Projeto