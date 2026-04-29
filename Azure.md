# Introdução à Infraestrutura de Nuvem: Descrever conceitos de nuvem
## Conceitos Básicos do Microsoft Azure
O Microsoft Azure é uma plataforma de nuvem versátil que oferece serviços para todo tipo de projeto, desde a hospedagem de sites simples até infraestruturas complexas com computação virtualizada. Além de armazenamento e bancos de dados, a plataforma disponibiliza tecnologias avançadas em IA e IoT. O foco principal desta série é fornecer a base sobre computação em nuvem, os principais serviços da Microsoft e as ferramentas de governança e conformidade.

<img width="1920" height="1080" alt="azure-services-diagram" src="https://github.com/user-attachments/assets/919cac03-74f6-459c-9ad4-7e3a93ed87a8" />

## O que são conceitos básicos do Azure?
O Azure Fundamentals é uma trilha de aprendizado estruturada para quem deseja iniciar no ecossistema da Microsoft Cloud. O conteúdo abrange serviços de computação, rede, armazenamento, segurança, governança e gestão, mesclando teoria com desafios práticos de TI. Não exige experiência técnica prévia, sendo ideal para construir uma base sólida em nuvem.

## Por que devo usar os conceitos básicos de Azure
O curso de Conceitos Básicos do Azure é o ponto de partida ideal tanto para iniciantes quanto para quem já tem experiência e busca a certificação oficial. Ele é estruturado para cobrir as três principais áreas do exame AZ-900, com pesos distribuídos da seguinte forma:

---
* **Arquitetura e Serviços do Azure (35-40%):** O foco principal, tratando da estrutura e funcionamento da nuvem Microsoft.
* **Gerenciamento e Governança (30-35%):** Ferramentas de controle e conformidade.
* **Conceitos de Nuvem (25-30%):** Fundamentos e benefícios gerais do modelo de nuvem.
---

É o roteiro essencial para quem deseja validar conhecimentos técnicos e obter uma compreensão abrangente da plataforma.

# O que é computação em nuvem
A computação em nuvem consiste na entrega de recursos de tecnologia — como servidores, armazenamento, redes e bancos de dados — via internet. Indo além da infraestrutura tradicional, ela engloba inovações como IA, Machine Learning e IoT.
O seu grande diferencial é a escalabilidade: por não estar presa às limitações físicas de um datacenter local, a nuvem permite expandir ou reduzir sua capacidade de TI de forma quase instantânea, eliminando a necessidade de grandes obras ou espera por hardware físico.

## Descrever o modelo de responsabilidade compartilhada
Talvez você tenha ouvido falar do modelo de responsabilidade compartilhada, mas talvez não entenda o que significa e como afeta na computação em nuvem.

## Como as responsabilidades se transformam na nuvem
O Modelo de Responsabilidade Compartilhada define quem faz o quê na nuvem, contrastando com o modelo tradicional (On-premises):
* **No Datacenter Local (On-premises):** Você é dono de tudo. É responsável desde a segurança física e energia até a atualização do sistema operacional e dos dados.
* **Na Nuvem:** A carga é dividida. O provedor (Microsoft) sempre cuida da infraestrutura física (segurança do prédio, energia, resfriamento). O consumidor (você) sempre cuida dos dados, das contas e da segurança de acesso.

**A Responsabilidade por Tipo de Serviço:**
A divisão do "meio do caminho" (como sistemas operacionais e rede) varia conforme o modelo escolhido:

* **IaaS (Infraestrutura como Serviço):** É onde você tem mais controle e mais trabalho. O provedor cuida do hardware, mas você cuida da VM, do sistema operacional e das atualizações.

* **PaaS (Plataforma como Serviço):** É o equilíbrio. O provedor gerencia o sistema operacional e o software base (como um banco de dados SQL), e você foca apenas na aplicação e nos dados.

* **SaaS (Software como Serviço):** É onde o provedor cuida de quase tudo. Você é apenas o usuário final do software, sendo responsável apenas pelos dados que insere e por quem tem acesso à conta.

**Regra de ouro:** Não importa o modelo (IaaS, PaaS ou SaaS), a responsabilidade pelos dados, dispositivos (endpoints) e gerenciamento de contas/identidades será sempre sua.







