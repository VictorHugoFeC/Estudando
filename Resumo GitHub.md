# Estudando GitHub

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
GitHub disponibiliza a opção de onde você quer receber essa notificação.
* **Email:** Notificação entregue no seu email registrado.
* **Web:** Notificação exibida diretamente no painel do GitHub.
* **Móvel:** Notificações por pucj usando o applicativo móvel GitHub.
* **Notificações personalizadas:** Configurações de tipos de evento específico para canais diferentes.













