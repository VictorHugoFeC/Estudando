# Estudando

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



