# VS Code

## Configurando o Git

Antes de começarmos a usar o Git pelo VS Code precisamos rodar dois comandos para nossa configuração.
Abra o terminal na pasta do repositório e digite:

```bash
git config --local user.name "Seu usuario"
git config --local user.email "Seu email"
```

## Criando um repósitorio

TODO
1 - Mover criando um repositório para a página inicial (repete o mesmo processo nas três pastas)

## Clonando um repositório

Após ter criado seu repositório vamos clona-lo usando o VS Code, para isso digite `Ctrl+Shift+P` e digite `Git clone`, depois escolha a opcao `Clone from GitHub`, um pop-up aparecerá, clique em `Allow` e logue na sua conta GitHub, um outro pop-up irá aparecer, clique em `Abrir Visual Studio Code - URL Handler` e depois `Open` no VSCode. Depois disso escolha o repositório que deseja clonar e selecione a pasta onde deseja clona-lo.

## Fazendo um commit


No VS Code digite `Ctrl+Shift+P` novamente e depois `Git Commit All` para fazer um commit com todos os arquivos que foram alterados dentro do repositório. Apos ter selecionado os comandos um novo arquivo aparecerá com alguns comentarios nele

![commit](/vscode/Images/commit.png)

Digite uma mensagem dando uma breve explicação sobre a alteração feita e feche o arquivo

![commit_message](/vscode/Images/commit_message.png)

Pronto, o commit já foi criado e agora precisamos manda-lo para o GitHub no repositório remoto. Digite `Ctrl+Shift+P` e `Git Push` e pronto seu commit foi enviado para o repositório remoto

TESTANDO GIT PULL
