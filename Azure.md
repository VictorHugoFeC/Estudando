# Introdução à Infraestrutura de Nuvem e Microsoft Azure

Este repositório contém anotações e conceitos fundamentais sobre computação em nuvem, focando no ecossistema **Microsoft Azure**. O conteúdo aqui descrito serve como base para a certificação **AZ-900 (Azure Fundamentals)**.

---

## Conceitos Básicos do Microsoft Azure

O **Microsoft Azure** é uma plataforma de nuvem versátil que oferece serviços para todo tipo de projeto: desde a hospedagem de sites simples até infraestruturas complexas com computação virtualizada. 

Além de armazenamento e bancos de dados, a plataforma disponibiliza tecnologias avançadas em **IA (Inteligência Artificial)** e **IoT (Internet das Coisas)**. Este guia foca em fornecer a base sobre:
* Principais serviços da Microsoft.
* Ferramentas de governança e conformidade.
* Modelos de computação em nuvem.

![Azure Services Diagram](https://github.com/user-attachments/assets/919cac03-74f6-459c-9ad4-7e3a93ed87a8)

### O que é o Azure Fundamentals?
É uma trilha de aprendizado estruturada para quem deseja iniciar no ecossistema da Microsoft Cloud. O conteúdo abrange:
- [x] Serviços de computação e rede.
- [x] Armazenamento e segurança.
- [x] Governança e gestão de custos.
- [x] Desafios práticos de TI.

### Por que estudar os fundamentos?
O curso é o ponto de partida ideal para iniciantes e profissionais que buscam a certificação oficial. O exame **AZ-900** é dividido em três áreas principais:

> | Área de Conhecimento | Peso no Exame |
> | :--- | :--- |
> | **Arquitetura e Serviços do Azure** | 35-40% |
> | **Gerenciamento e Governança** | 30-35% |
> | **Conceitos de Nuvem** | 25-30% |

---

## O que é Computação em Nuvem?

A computação em nuvem consiste na entrega de recursos de tecnologia — como servidores, armazenamento, redes e bancos de dados — via internet. 

**Diferencial Chave: Escalabilidade**
Ao contrário de um datacenter local, a nuvem permite expandir ou reduzir a capacidade de TI quase instantaneamente, eliminando a necessidade de hardware físico próprio ou grandes investimentos iniciais.

---

## Modelo de Responsabilidade Compartilhada

Um dos conceitos mais importantes na nuvem é entender "quem é responsável pelo quê". Esse modelo define a divisão de tarefas entre você (o consumidor) e a Microsoft (o provedor).

### A transformação das responsabilidades
* **On-premises (Local):** Você é responsável por tudo (desde a energia do prédio até os dados).
* **Na Nuvem:** A carga é dividida. A Microsoft cuida da segurança física, energia e hardware.

### Responsabilidade por Modelo de Serviço

Abaixo, veja como a responsabilidade muda conforme o modelo escolhido:

1.  **IaaS (Infraestrutura como Serviço):** Maior controle. O provedor cuida do hardware; você cuida da VM, do SO e das atualizações.
2.  **PaaS (Plataforma como Serviço):** Equilíbrio. O provedor gere o SO e o software base; você foca na aplicação e nos dados.
3.  **SaaS (Software como Serviço):** Conveniência total. O provedor cuida de quase tudo; você gerencia apenas seus dados e acessos.

![Shared Responsibility Model](https://github.com/user-attachments/assets/ab6145bf-fa62-470e-8d3f-4c9c66ae08f4)

### Check-list de Responsabilidades

| Ativo | Responsabilidade do Usuário | Responsabilidade do Provedor |
| :--- | :---: | :---: |
| **Dados e Informações** | ✅ | ❌ |
| **Dispositivos (Endpoints)** | ✅ | ❌ |
| **Contas e Identidades** | ✅ | ❌ |
| **Datacenter Físico** | ❌ | ✅ |
| **Rede Física / Hosts** | ❌ | ✅ |
| **SO / Aplicativos** | *Depende do modelo (IaaS/PaaS)* | *Depende do modelo* |

> **Regra de Ouro:** Não importa o modelo (IaaS, PaaS ou SaaS), a responsabilidade pelos **dados**, **dispositivos** e **gerenciamento de identidades** será SEMPRE sua.

---
*Repositório criado para fins de estudo e documentação da jornada Cloud.*


