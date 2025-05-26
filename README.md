# Arquiteturas_Azure

☁️ Construindo Arquiteturas no Azure

Este projeto tem como objetivo demonstrar, de forma prática e didática, como construir uma arquitetura sólida e segura na nuvem da **Microsoft Azure**, abordando desde a criação de recursos fundamentais até aspectos de controle, segurança e organização.

Você entenderá como se concentram os componentes essenciais da arquitetura no Azure, incluindo redes, controle de acesso, organização de recursos e boas práticas relacionadas à disponibilidade e gerenciamento.

---

## 🌎 Região e Disponibilidade no Brasil

Os recursos deste projeto são implantados em **regiões brasileiras do Azure**, como:

- **Brazil South** (Estado de São Paulo)
- **Brazil Southeast** (Estado do Rio de Janeiro)

Essas regiões garantem **baixa latência**, **conformidade local** com a LGPD, e **alta disponibilidade**, com múltiplas zonas de disponibilidade (quando suportado). A escolha da região influencia diretamente no desempenho, custo e tolerância a falhas da aplicação.

---

## 🖥️ Visão Geral da Sala de Servidores (Datacenter)

Embora a nuvem seja virtual, os datacenters físicos existem. No caso do Azure no Brasil, os dados ficam armazenados em instalações seguras, climatizadas, com monitoramento constante, controle de acesso rígido e redundância de energia e rede, garantindo disponibilidade de **99,9% ou mais**, dependendo do serviço.

---

## 📌 Recursos Práticos Criados

Durante o projeto, abordamos a criação e validação dos seguintes componentes:

### ✅ Grupo de Recursos
- Criar um **Resource Group** para centralizar recursos relacionados a uma mesma aplicação ou ambiente.
- Importância para organização e gerenciamento de custos.

### 🕵️‍♂️ Log de Atividades
- Acompanhamento de **ações realizadas** no ambiente Azure.
- Ideal para auditoria e rastreamento de mudanças.

### 👥 IAM (Controle de Acesso)
- Gerenciamento de **permissões baseadas em funções (RBAC)**.
- Controle detalhado sobre quem pode visualizar, modificar ou administrar recursos.

### 🏷️ Marcações (Tags)
- Adição de **tags** para facilitar a organização, rastreamento de custos e automações.
  - Ex: `Projeto=ArquiteturaAzure`, `Ambiente=Desenvolvimento`, `Responsável=Humberto`.

### 📄 Propriedades
- Consulta de informações gerais sobre os recursos (ID, localização, status).

### 🔒 Bloqueios (Locks)
- Aplicação de bloqueios de **exclusão ou modificação** para evitar alterações acidentais em recursos críticos.

### 🎉 Eventos (Event Grid / Monitor)
- Monitoramento e reação a eventos no ambiente (criação de recurso, alertas, etc.).

---

## 🌐 Criar Rede Virtual

Foi criada uma **Virtual Network (VNet)** para isolar e proteger os recursos da nuvem:

- Sub-redes (subnets) organizadas por função (ex: app, banco de dados)
- Configurações de DNS, NSG (grupo de segurança de rede) e endereçamento IP interno
- Base para futuras integrações com VPN, ExpressRoute e aplicações distribuídas
