# Introdução ao Git

## O que é controle de versão?
Um VCS(sistema de controle de versão) é um programa ou um conjunto de programas que controla alterações feitas em uma coleção de arquivos. Facilitando recuperar versões anteriores e dando acesso simultâneo aos usuários ou membros sem afetar o arquivo. O VCS é tecnicamente, uma das práticas envolvidas no SCM(gerenciamento de configurações de software), mas o VCS pode ser usado para projetos além de software, incluindo manuais e tutoriais online. Git é um VCS rápido, versátil, altamente escalonável, gratuito e de software livre, o autor principal é Linus Torvalds, o criador do Linux.

## Terminologia do Git
A seguir uma breve lista dos termos usados com frequência pelos usuários do Git.
* **Árvore de trabalho:** O conjunto de diretórios aninhados e arquivos que contêm o projeto em que está sendo trabalhado.
* **Repositório:** O diretório, localizado no nível superior de uma árvore de trabalho, onde o Git mantém todo o histórico e os metadados de um projeto.
* **Hash:** No Git, nada é rastreado pelo nome do arquivo, mas sim pelo seu conteúdo. O Hash é uma sequência alfanumérica única (ex: a1b2c3d...) gerada por um algoritmo. É o "RG" de cada alteração. Se você mudar um único espaço em um arquivo, o Hash será completamente diferente. Isso garante a integridade dos dados.
* **Objeto(Object):** O Git armazena tudo em um banco de dados de objetos. Existem quatro tipos principais:
  * Blob: Armazena o conteúdo dos arquivos.
  * Tree: Funciona como uma pasta, agrupando Blobs e outras Trees.
  * Commit: Aponta para uma Tree e contém metadados (autor, data, mensagem).
  * Tag: Um rótulo fixo para um commit específico.
* **Commit:** Um Commit é como um "checkpoint" ou uma foto (snapshot) do seu projeto naquele exato momento. Diferente de outros sistemas que salvam apenas as diferenças, o Git salva o estado completo dos arquivos. Se um arquivo não mudou, ele apenas cria um link para a versão anterior para economizar espaço.
* **Branch(Ramo):** Uma Branch é simplesmente um ponteiro móvel para um commit. A branch padrão geralmente se chama main ou master. Criar uma branch permite que você trabalhe em uma nova funcionalidade sem "quebrar" o código principal. É como criar uma linha do tempo paralela.
* **Remoto(Remote):** O Remoto é a versão do seu projeto que está hospedada na internet ou em um servidor (como GitHub, GitLab ou Bitbucket). Origin: É o nome padrão dado ao servidor remoto de onde você clonou o projeto.
* **Comandos Essenciais:** Para colocar essa terminologia em prática, usamos os comandos no terminal:
  * **git init:** Inicializa um novo repositório Git local na pasta atual.
  * **git clone [url]:** Baixa um projeto existente de um servidor remoto para o seu computador.
  * **git status:** Exibe o estado atual do diretório de trabalho (quais arquivos foram modificados ou adicionados).
  * **git add [arquivo]:** Adiciona arquivos específicos à Staging Area (preparação). Use git add . para adicionar tudo.
  * **git commit -m "mensagem":** Grava o snapshot dos arquivos que estão na Staging Area permanentemente no histórico.
  * **git branch:** Lista as branches existentes. Use git branch [nome] para criar uma nova.
  * **git checkout [nome-da-branch]:** Alterna para a branch especificada (ou git switch).
  * **git merge [nome-da-branch]:** Une o histórico da branch especificada à branch atual.
  * **git remote add origin [url]:** Conecta seu repositório local a um servidor remoto.
  * **git push origin [branch]:** Envia seus commits locais para o servidor remoto.
  * **git pull:** Atualiza seu repositório local com as alterações que estão no servidor remoto.
  * **git log:** Mostra o histórico de todos os commits realizados no projeto.


# Introdução ao GitHub

## O que são gists?
Permite que o usuário compartilhe snippets de código, anotações ou outroas pequenas informações. São mini 
repositórios do Git, fazendo o papel de um repositório mas com soluções rápidas.

## Principais recursos de Gists

* **Gists públicos e secretos:**
Gists públicos são visíveis para todos, com o objetivo de compartilha snippets de cósigo ara comunidade ampla.
Gists secretos podem ser pesquisados mas apenas pessoas com acesso a URL podem acessar(limitando acesso).

* **Controle de versão:**
Cada alteração feita é salva, e possibilitando acesso a alterações anteriores. (Victor pensa em um BD)

* **Fork e Clonagem:**
Como repositórios, os gists podem ser bifurcados e clonados.

* **Inserindo:**
Os gists podem ser inseridos em sites ou blogs, sendo uma ótima ferramenta como códigos em tutoriais ou documentação.

* **Suporte ao Markdown:**
Embora os Gists normalmente são usados para snippets individuais, eles também podem ser compartilhados e colaborados por vários usuários.

## Componentes do fluxo do GitHub (conceitos fundamentais do Git)

### O que são branches?
Branches são essencial, eles permitem fazer alterações sem alterar o branch padrão. É um lugar seguro para experimentar coisas novas,
recursos ou até correções.

### O que são commits?
Commits estão relacionados a uma trilha fornecida como se fosse uma revisão de histórico de um arquivo vinculado.

### Arquivos Git Não Rastrados e Rastreados.
Não rastreados é quando ele ainda não faz parte do repositório Git. Já os Rastrados são aqueles que estão sendo monitorados pelo
Git ativamente, a entidade pode estar nos seguintes subestados:
* **Não modificado:** O arquivo é rastrado mas não foi modificado desde a última confirmação.
* **Modificado:** O arquivo foi alterado desde o último commit, mas as alterações não foram para o próximo commit.
* **Preparado:** O arquivo foi modificado e foi adicionado na área de preparo(conhecida como índice).
* **Comitado:** O arquivo está no Bd do repositório, ele representa a versão mais recente desse repositório.

## O que são pull requests?
Uma soçicitação de pull é o mecanismo usado para sinalizar as confirmações de um branch pronto para ser mesclado com outro brench.

## O fluxo do GitHub
* **Criar o branch "feature" de "main":** Começar criando um branch para que suas alterações, recursos ou correções não afetem o branch principal.
* **Confirmar as alterações:** Em seguida, faça suas atualizaações na ramificação. Teste a ramificação antes de realizar a implementação.
* **Enviar uma Solicitação de Pull:** Agora, abra um pull request para solicitar um feedback e começar uma revisão.
* **Discutir as alterações propostas:** Em seguida, examine comentários e faça atualizações necessárias com base nos comentários da sua equipe.
* **Mesclar o branch "feature" no "main":** Por fim, dhttps://github.com/VictorHugoFeC/Estudando/projectsepois da mudança, receba aprovação e mescle a solicitação de pull na ramificação principal. Depois disso,
exclua a ramificação para manter seu repositório limpo e evitar ramificações desatualizadas.

## Fluxo Git: tipos de ramificação 
O fluxo do git usa várias ramificações temporárias e de longa duração:
* **master:** Sempre reflete o código pronto para o ambiente de produção.
* **desenvolvimento:** Contém o trabalho de desenvolvimento mais recente para a próxima versão.
* **feature/:** Utlizado para criar novos recursos; ramificado a partir de develop e depois mesclado novamente quando concluído.
* **release/:** Prepara uma nova versão de produção de develop, permite testes finais e pequenas correções de bug.
* **hotfix/:** Usado para corrigir rapidamente problemas de produção; ramificado de master.

## Discussão
Já dentro do repositório selecione Discussões na parte de cima do GitHub, click nova discussão, crie com a categoria que você deseja, coloque o título do tema que vai ser abordado, descreva sobre o problema na caixa de texto e pronto, outros usuários podem fazer comentários sobre o seu telma levantado, uma ferramenta  ótima para ter um canal de contato direto com os usuários dentro do projeto do GitHub.

## Notficações
GitHub permite que você filtre notificações usando configurações de acompanhamento.
* **Observando:** Recebe notficações de todas as atividades.
* **Nçao assistindo:** Receba notificações apenas quando estiver participando ou @mentioned.
* **Ignorar:** Nenhuma notificação para um repositório.
* **Personalizado:** Ajuste quais stipos de atividades(Como solicitação de pull, problemas ou discussões) disparam notificações.
---
GitHub disponibiliza a opção de onde você quer receber essa notificação.
* **Email:** Notificação entregue no seu email registrado.
* **Web:** Notificação exibida diretamente no painel do GitHub.
* **Móvel:** Notificações por pucj usando o applicativo móvel GitHub.
* **Notificações personalizadas:** Configurações de tipos de evento específico para canais diferentes.

## Introdução aos produtos do GitHub
GitHub para Dispositivos Móveis e GitHub para Desktop e acessar seu GitHub pelo site da web github.com

## GitHub Mobile
GitHub está disponível para Android e IOS, podendo ser acessado de qualqur lugar com o seu dispositivo de maneira segura e protejida, criado pela própria plataforma. O GitHub Mobile vai te auxiliar com as notificações, pesquisar e navegar interagindo com os usuários, e até executar tarefas leves.

## GitHub Desktop
GitHub está disponível para Windows e macOS, é um aplicativo que simplifica o fluxo de trabalho do Git, ajudando na interação entre as colaborações, compartilhamento de boas práticas do Git e do GitHub dentro da sua equipe. Adicionar repositórios é uma das funções que o aplicativo no Desktop tem, além de clonar repositório, adicionar alterações e muito mais.

## Cobrança do GitHub
GitHub cobra contas com base no tipo: pessoal, organização ou enterprise. Cada cobrança reflete uma combinação de assinaturas e cobranças baseadas em uso: 
* **Assinaturas** incluem o plano da sua conta(como GitHub Pro ou GitHub Team) e custos mensais fixos para produtos como GitHub Copilot ou aplicativos do Marketplace.
* **Cobrança baseada em uso** se o aplicativo cujo custo aumenta com o uso, como GitHub Actions (baseado em minutos de runtime e armazenamento de artefatos) ou GitHub Packges. 












