# Fluxo de trabalho no repositório
- [Fluxo de trabalho no repositório](#fluxo-de-trabalho-no-repositório)
  - [Pré requisito](#pré-requisito)
  - [Fluxo](#fluxo)
    - [1 - Baixe o repositório na sua máquina](#1---baixe-o-repositório-na-sua-máquina)
    - [2 - Crie uma branch a partir da branch `next`](#2---crie-uma-branch-a-partir-da-branch-next)
    - [3 - Faça o seu trabalho e crie um `commit` com as mudanças sempre que possível](#3---faça-o-seu-trabalho-e-crie-um-commit-com-as-mudanças-sempre-que-possível)
    - [4 - Terminou? Agora é a hora de criar uma *pull request* para a *branch* `next`](#4---terminou-agora-é-a-hora-de-criar-uma-pull-request-para-a-branch-next)
    - [5 - Chame o time para revisar a tarefa](#5---chame-o-time-para-revisar-a-tarefa)
    - [6 - Depois de aprovada a *pull request*, é hora de incluir ela para a `next`!](#6---depois-de-aprovada-a-pull-request-é-hora-de-incluir-ela-para-a-next)
## Pré requisito

Este guia segue o fluxo para a utilização via interface gráfica e para isso você precisa instalar o [Github desktop](https://desktop.github.com/). 

Se você prefere utilizar via terminal, siga o [tutorial Fluxo de trabalho no repositório - via terminal](./../CONTRIBUTING.md).

## Fluxo

### 1 - Baixe o repositório na sua máquina

Ao instalar o github desktop e fazer login no github, irá aparecer uma janela inicial com uma lista de acoes. Para baixar o repositório do `pods-design`, clique no botão "Clone a Repository from the internet...".

![Janela do github actions contendo as acoes iniciais](./../assets/img/github-desktop/clone.png)

Ao clicar, irá abrir uma janela para pesquisar o nome do repositório, e ao digitá-lo, irá aparecer para voce uma lista contendo `po-ds/pods-design`.

![Janela para pesquisar o repositório que se deseja baixar](./../assets/img/github-desktop/clone-2.png)

Depois de baixar, irá aparecer uma janela que futuramente será mostrado as alteracões que vão aparecer no arquivo.

![alt](./../assets/img/github-desktop/clone-3.png)

### 2 - Crie uma branch a partir da branch `next`

Garanta que o seu respositório local esteja atualizado da seguinte forma, parte superior, clique na aba "Repository" e em seguida em 
"Pull":

![alt](./../assets/img/github-desktop/pull.png)

Agora vamos criar a branch:

![alt](./../assets/img/github-desktop/branch.png)

![alt](./../assets/img/github-desktop/branch-2.png)

Dessa forma, uma nova branch será criada a partir da `next`.

### 3 - Faça o seu trabalho e crie um `commit` com as mudanças sempre que possível

![alt](./../assets/img/github-desktop/commit.png)

Depois de fazer o commit da sua alteracao é necessário enviá-lo ao servidor. Para isso precisamos fazer o "push" dos commits. 

Mas no seu primeiro push, vai ser necessário publicar a branch, para que ela esteja disponível no servidor para os outros usuários. 

![alt](./../assets/img/github-desktop/commit-2.png)

Depois disso podemos fazer o push:

![alt](./../assets/img/github-desktop/push.png)

### 4 - Terminou? Agora é a hora de criar uma *pull request* para a *branch* `next`

Entre na página de [pull requests do PODS](https://github.com/po-ds/pods-design/pulls). E clique no botão escrito "New pull request", conforme a imagem abaixo.

![página de criação de pull request](./../assets/img/create-pr.png)

Depois você precisa configurar a *pull request*, da seguinte maneira:

1. Escolha a branch `next` como *base* e a sua *branch* atual como *compare*. 

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
