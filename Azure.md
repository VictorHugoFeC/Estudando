# Introdução à Infraestrutura de Nuvem e Microsoft Azure

Este repositório contém anotações e conceitos fundamentais sobre computação em nuvem, focando no ecossistema **Microsoft Azure**. O conteúdo aqui descrito serve como base para a certificação **AZ-900 (Azure Fundamentals)**.

---

## ☁️ Conceitos Básicos do Microsoft Azure

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

| Área de Conhecimento | Peso no Exame |
| :--- | :--- |
| **Arquitetura e Serviços do Azure** | 35-40% |
| **Gerenciamento e Governança** | 30-35% |
| **Conceitos de Nuvem** | 25-30% |

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
1.  **IaaS (Infraestrutura como Serviço):** Maior controle. O provedor cuida do hardware; você cuida da VM, do SO e das atualizações.
2.  **PaaS (Plataforma como Serviço):** Equilíbrio. O provedor gere o SO e o software base; você foca na aplicação e nos dados.
3.  **SaaS (Software como Serviço):** Conveniência total. O provedor cuida de quase tudo; você gerencia apenas seus dados e acessos.

![Shared Responsibility Model](https://github.com/user-attachments/assets/ab6145bf-fa62-470e-8d3f-4c9c66ae08f4)

### Check-list de Responsabilidades

| Ativo | Usuário | Provedor |
| :--- | :---: | :---: |
| **Dados e Informações** | ✅ | ❌ |
| **Dispositivos (Endpoints)** | ✅ | ❌ |
| **Contas e Identidades** | ✅ | ❌ |
| **Datacenter Físico** | ❌ | ✅ |
| **Rede Física / Hosts** | ❌ | ✅ |
| **SO / Aplicativos** | *IaaS / PaaS* | *PaaS / SaaS* |

> [!IMPORTANT]
> **Regra de Ouro:** Não importa o modelo (IaaS, PaaS ou SaaS), a responsabilidade pelos **dados**, **dispositivos** e **gerenciamento de identidades** será SEMPRE sua.

---

## Modelos de Implantação de Nuvem

Modelos de nuvem definem o tipo de implantação de recursos. A escolha depende das necessidades de controle, custo e escalabilidade.

<img width="100%" alt="cloud-deployment-models" src="https://github.com/user-attachments/assets/1d535ea7-2ce3-47cb-ad9e-b5b1463f162c" />

### 1. Nuvem Privada (Private Cloud)
Ambiente usado exclusivamente por uma única entidade.
* **Vantagem:** Controle total sobre a segurança e os dados.
* **Desvantagem:** Custos elevados de manutenção e hardware (CapEx).
* **Onde fica:** Datacenter local (on-premises) ou hospedada por terceiros em hardware dedicado.

### 2. Nuvem Pública (Public Cloud)
Criada, controlada e mantida por um provedor (ex: Microsoft, AWS, Google). 
* **Vantagem:** Sem custos iniciais de hardware; modelo de pagamento por uso (Pay-as-you-go).
* **Acesso:** Disponível para qualquer pessoa via internet.
* **Diferencial:** Escalabilidade quase infinita e alta disponibilidade.

### 3. Nuvem Híbrida (Hybrid Cloud)
Um ambiente interconectado que combina nuvens públicas e privadas.
* **Flexibilidade:** Permite o *Cloud Bursting* (escalar para a pública em picos de demanda).
* **Segurança:** Mantém dados sensíveis no privado e aplicações de larga escala no público.

---

## Comparativo: Público vs. Privado vs. Híbrido

| Característica | Nuvem Pública | Nuvem Privada | Nuvem Híbrida |
| :--- | :--- | :--- | :--- |
| **Custo Inicial (CapEx)** | Praticamente zero | Alto | Variável |
| **Manutenção** | Provedor | Organização | Compartilhada |
| **Escalabilidade** | Altíssima e rápida | Limitada ao hardware | Flexível |
| **Controle/Segurança** | Padrão do provedor | Total e personalizado | Personalizado |

---

## Cenários Avançados e Integração

### Multicloud (Várias Nuvens)
Uso de múltiplos provedores de nuvem pública (ex: usar Azure para IA e AWS para armazenamento) para evitar dependência de um único fornecedor (*vendor lock-in*).

### Azure Arc
O **Azure Arc** é o "braço operacional" que unifica a gestão de recursos em ambientes diversos:
- [x] **Nuvem Pública** (Apenas Azure).
- [x] **Nuvem Privada** (Seu próprio datacenter).
- [x] **Nuvem Híbrida** (Conexão local + Azure).
- [x] **Multicloud** (Gerenciar AWS ou Google Cloud dentro do portal do Azure).

### Solução VMware no Azure (AVS)
Ideal para empresas que já utilizam VMware localmente e desejam migrar sem reescrever aplicações.
* **Integração:** Execute cargas de trabalho VMware nativamente no Azure.
* **Gestão:** Mantém as ferramentas conhecidas pela equipe técnica.

---

### Resumo de Conceitos-Chave

> | Termo | O que você não pode esquecer |
> | :--- | :--- |
> | **Multicloud** | Uso de múltiplos provedores públicos. |
> | **Azure Arc** | Ponte de gerenciamento para ambientes híbridos e multinuvem. |
> | **VMware no Azure** | Migração suave de ambientes VMware locais para o Azure. |

---
*Repositório criado para fins de estudo e documentação da jornada Cloud.*

# Introdução à Extração de Informações com IA no Microsoft Azure

O ecossistema de **Serviços de IA do Azure** oferece uma ampla gama de soluções baseadas em nuvem para tarefas de inteligência artificial, permitindo a extração e análise sistemática de informações a partir de conteúdos digitais.

## Principais Serviços

Os serviços abaixo são os pilares para cenários de extração de dados e análise inteligente:

* **Azure AI Vision (Análise de Imagem):** Permite extrair insights de imagens, incluindo a detecção e identificação de objetos, geração de legendas (captions), marcas relevantes (tags) e extração de texto (OCR).
* **Azure AI Content Understanding (Compreensão de Conteúdo):** Um serviço de análise multimodal que extrai insights de documentos estruturados, imagens, áudio e vídeo de forma unificada.
* **Azure AI Document Intelligence (Inteligência de Documentos):** Projetado para extrair campos e valores de formulários digitais ou digitalizados, como faturas, recibos, pedidos de compra e documentos de identidade.
* **Azure AI Search (Pesquisa de IA):** Executa indexação assistida por IA através de um pipeline de habilidades, permitindo pesquisar informações sistematicamente em conteúdos estruturados e não estruturados.

---

> [!IMPORTANT]
> Você pode utilizar esses serviços separadamente ou combiná-los para criar soluções personalizadas e robustas.












