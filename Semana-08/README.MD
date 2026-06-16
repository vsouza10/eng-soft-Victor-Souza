# Documento de Requisitos de Software (SRS)

## Informações do Projeto

| Campo | Descrição |
|---------|---------|
| Nome do Projeto | Sistema de Gestão de Reservas - Hotel Bela Vista |
| Dono do Projeto | Hotel Bela Vista |
| Versão | 1.0 |
| Data | 16/04/2026 |

---

# 1. Introdução

Este documento descreve os requisitos do sistema de gerenciamento de reservas do Hotel Bela Vista.

---

# 2. Escopo

O sistema terá como objetivo:

- Funcionalidade 1: Gerenciar reservas.
- Funcionalidade 2: Controlar ocupação dos quartos.
- Funcionalidade 3: Registrar consumo dos hóspedes.
- Funcionalidade 4: Facilitar a visualização da situação do hotel.

---

# 3. Requisitos Funcionais

## 3.1 Funcionalidade 1

| ID | Descrição do Requisito |
|------|------|
| RF 1.1 | O sistema deve exibir um painel com todos os quartos e seus status (livre, ocupado e limpeza). |
| RF 1.2 | O sistema deve permitir o cadastro de reservas. |
| RF 1.3 | O sistema deve impedir reservas duplicadas para o mesmo quarto no mesmo período. |
| RF 1.4 | O sistema deve permitir o cadastro completo de hóspedes (nome, telefone e CPF). |
| RF 1.5 | O sistema deve exibir entradas e saídas do dia. |
| RF 1.6 | O sistema deve permitir o registro de consumo por hóspede. |
| RF 1.7 | O sistema deve calcular automaticamente o valor total no checkout. |

---

# 4. Requisitos Não Funcionais

- **RNF01:** O sistema deve ser acessível via computador.
- **RNF02:** O sistema deve possuir interface simples e intuitiva.
- **RNF03:** O sistema deve responder em até 2 segundos.

---

# 5. Design da Interface do Usuário (UI)

## Design 1

O sistema terá uma interface simples e intuitiva, com uso de cores para representar o status dos quartos:

- 🟢 Verde: disponível
- 🔴 Vermelho: ocupado
- 🟡 Amarelo: em limpeza

A interface será acessada via navegador, com layout focado em tela desktop.

## Design 2

Fluxo principal do sistema:

```text
Login
 ↓
Painel de Quartos
 ↓
Seleção de Quarto
 ↓
Cadastro/Visualização de Reserva
 ↓
Checkout
```

O sistema será projetado para uso rápido, com poucas etapas e navegação direta.

---

# 6. Arquitetura do Sistema

## Arquitetura 1

O sistema utilizará arquitetura em camadas (MVC), separando:

- Interface
- Lógica de Negócio
- Dados

## Arquitetura 2

### Front-end

- HTML
- CSS
- JavaScript

### Back-end

- PHP

### Banco de Dados

- MySQL

### Servidor Local

- XAMPP

---

# 7. Requisitos de Dados

## RD 7.1 – Principais Entidades

- Hóspede
- Quarto
- Reserva
- Consumo

### Relacionamentos

- Um hóspede pode ter várias reservas.
- Um quarto pode ter várias reservas em períodos diferentes.
- Uma reserva pode ter vários consumos.

## RD 7.2 – Regras de Dados

- Nome do hóspede obrigatório.
- CPF do hóspede obrigatório.
- Não permitir reservas duplicadas no mesmo período.
- Backup manual periódico do banco de dados.

---

# 8. Requisitos de Segurança

- **RS 8.1:** O sistema terá autenticação por login e senha para acesso dos funcionários.
- **RS 8.2:** O sistema utilizará HTTPS para comunicação segura e proteção básica dos dados.

---

# 9. Requisitos de Desempenho

- **RP 9.1:** Especificação de throughput e suporte a acessos simultâneos.
- **RP 9.2:** Limites de consumo de memória e processamento em ambiente de produção.

---

# 10. Requisitos de Teste

- **RT 10.1:** Estratégia para testes unitários, testes de integração e cobertura de código.
- **RT 10.2:** Procedimentos para testes de aceitação do usuário (UAT) e critérios de sucesso.

---

# 11. Cronograma do Projeto

| Tarefa | Data de Início | Data de Término |
|---------|---------|---------|
| Levantamento de Requisitos | 10/04 | 12/04 |
| Design e Prototipagem | Ajustes Futuros | [Data] |
| Desenvolvimento | Ajustes Futuros | [Data] |
| Testes | Ajustes Futuros | [Data] |
| Implantação | Ajustes Futuros | [Data] |

---

# Revisões

| Versão | Data | Descrição |
|---------|---------|---------|
| 1.0 | 16/04 | Versão inicial |
| 1.1 | Ajustes Futuros | Atualização dos requisitos funcionais baseada no feedback inicial |

---

# Assinaturas

**Dono do Projeto:** Geraldo

________________________________________

**Gerente de Projeto:** Victor Emanuel de Souza

________________________________________
