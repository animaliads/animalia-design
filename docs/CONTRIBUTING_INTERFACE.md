# Fluxo de trabalho no repositório - interface gráfica
- [Fluxo de trabalho no repositório - interface gráfica](#fluxo-de-trabalho-no-repositório---interface-gráfica)
  - [Pré requisito](#pré-requisito)
  - [Fluxo](#fluxo)
    - [1 - Baixe o repositório na sua máquina](#1---baixe-o-repositório-na-sua-máquina)
    - [2 - Crie uma *branch* a partir da *branch* `next`](#2---crie-uma-branch-a-partir-da-branch-next)
    - [3 - Faça o seu trabalho e crie um `commit` com as mudanças sempre que possível](#3---faça-o-seu-trabalho-e-crie-um-commit-com-as-mudanças-sempre-que-possível)
    - [4 - Terminou? Agora é a hora de criar uma *pull request* para a *branch* `next`](#4---terminou-agora-é-a-hora-de-criar-uma-pull-request-para-a-branch-next)
    - [5 - Chame o time para revisar a tarefa](#5---chame-o-time-para-revisar-a-tarefa)
    - [6 - Depois de aprovada a *pull request*, é hora de incluir ela para a `next`!](#6---depois-de-aprovada-a-pull-request-é-hora-de-incluir-ela-para-a-next)
## Pré requisito

Este guia segue o fluxo para a utilização via interface gráfica e para isso você precisa instalar o [Github desktop](https://desktop.github.com/). 

Se você prefere utilizar via terminal, siga o [tutorial Fluxo de trabalho no repositório - via terminal](./../CONTRIBUTING.md).

## Fluxo

### 1 - Baixe o repositório na sua máquina

Ao instalar o Github desktop e fazer login no github, irá aparecer uma janela inicial com uma lista de ações. Para baixar o repositório do `pods-design`, clique no botão "Clone a Repository from the internet...".

![Janela do github actions contendo as acoes iniciais](./../assets/img/github-desktop/clone.png)

Ao clicar, irá abrir uma janela para pesquisar o nome do repositório, e ao digitá-lo, irá aparecer para você uma lista contendo `po-ds/pods-design`.

![janela para pesquisar o repositório que se deseja baixar](./../assets/img/github-desktop/clone-2.png)

Depois de baixar, irá aparecer uma janela que futuramente será mostrado as alterações que vão aparecer no arquivo.

![página principal contendo as mundaças nos arquivos e as ações](./../assets/img/github-desktop/clone-3.png)

### 2 - Crie uma *branch* a partir da *branch* `next`

Garanta que o seu respositório local esteja atualizado. Na parte superior, clique na aba "Repository" e em seguida em 
"Pull":

![dropdown superior contendo uma lista de ações para o respositório](./../assets/img/github-desktop/pull.png)

Agora vamos criar a *branch*, clicando no botão superior escrito "Current Branch", depois clique no botão "New Branch":

![página principal com o menu superior circulando o botão Current Branch](./../assets/img/github-desktop/branch.png)

Agora basta colocar o nome da nova *branch* e selecionar `next`, para que ela seja
criada a partir da `next`:

![janela de criação da nova branch com campo de entrada para o nome e campo de seleção para branch de origem](./../assets/img/github-desktop/branch-2.png)

Dessa forma, agora a sua *branch* foi criada localmente.

### 3 - Faça o seu trabalho e crie um `commit` com as mudanças sempre que possível

Nesta fase, você pode selecionar quais arquivos você quer que esteja no commit. 
Também pode adicionar um título para o commit e uma descrição, que servirão como uma
forma de rastreamento das alterações.

![página principal contendo as alterações no arquivo e os campos para preenchimento do commit](./../assets/img/github-desktop/commit.png)

Depois de fazer o commit da sua alteração é necessário enviá-lo ao servidor. Para isso precisamos fazer o "push" dos commits (enviar os commits para o servidor). 

Mas no seu primeiro "push", vai ser necessário publicar a *branch*, para que ela esteja disponível no servidor para os outros usuários. 

![página principal contendo um botão destacado escrito Publish branch](./../assets/img/github-desktop/commit-2.png)

Depois disso podemos fazer o push:

![página principal contendo um botão destacado escrito Push origin](./../assets/img/github-desktop/push.png)

### 4 - Terminou? Agora é a hora de criar uma *pull request* para a *branch* `next`

Entre na página de [pull requests do PODS](https://github.com/po-ds/pods-design/pulls). E clique no botão escrito "New pull request", conforme a imagem abaixo.

![página de criação de pull request](./../assets/img/create-pr.png)

Depois você precisa configurar a *pull request*, da seguinte maneira:

1. Escolha a *branch* `next` como *base* e a sua *branch* atual como *compare*. 

2. Adicione o título da *pull request*.

3. Adicione uma descrição. E direcione nesta descrição o que precisa ser revisado e como isso pode ser feito.

4. Clique no botão "Create pull request" para criar a pull request.
![página contendo o template para criar a pull request](./../assets/img/pr.png)

### 5 - Chame o time para revisar a tarefa

Nesse momento, compartilhe o link da sua *pull request* com as pessoas responsáveis por revisar.
Nesta revisão, essas pessoas poderão: aprovar, requisitar mudanças ou apenas comentar.
Para isso o Github tem uma documentação que explica [como aprovar pull requests](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/approving-a-pull-request-with-required-reviews).

### 6 - Depois de aprovada a *pull request*, é hora de incluir ela para a `next`!

Neste momento, você precisa alterar a opção "Merge pull request" para "Squash and merge". 

![botão para finalizar a pull request escrito "squash and merge"](./../assets/img/merge-pr.png)

Esta opção faz com que você resuma todos os *commits* da sua *pull request* em um único *commit*. Com isso irá abrir uma opção para você editar as mensagens de *commit*. 

![página para edição das mensagens de commit, transformando em um único commit](./../assets/img/squash-commit.png)

> Utilizar as regras de [descrição do commit descritas no Notion](https://www.notion.so/Conven-o-de-mensagens-de-commit-para-design-df19f55c6e6e48778d4a715ed70d23f1).
