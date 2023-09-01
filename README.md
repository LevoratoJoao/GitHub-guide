# Git e GitHub guide

Este repositorio é um guia inicial para quem quer aprender a usar Git e GitHub, nele você vai aprender comandos basicos para poder organizar seus projetos e trabalhos :)

<!--![GitHub_meme](https://github.com/LevoratoJoao/GitHub-guide/assets/90461798/b590945d-f8ea-4f78-b2e2-84740e607258)-->
<p align="center">
    <img width="400" src="https://github.com/LevoratoJoao/GitHub-guide/assets/90461798/b590945d-f8ea-4f78-b2e2-84740e607258" alt="GitHub Meme">
</p>

Primeiro, crie uma conta no [GitHub](https://github.com/signup), se você ainda não tem uma.

## O que é Git?

Git é um sistema de controle de versão distribuído, usado principalmente no desenvolvimento de software, mas pode ser usado para registrar o histórico de edições de qualquer tipo de arquivo.

## O que é GitHub?

GitHub é uma plataforma de hospedagem de código-fonte com controle de versão usando o Git. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou Open Source de qualquer lugar do mundo.

## Instalação

### Windows

TODO

### Linux

Abra o terminal e digite:

```bash
sudo apt-get install git
```
Para verificar se a instalação foi bem sucedida, digite:

```bash
git --version
```

## Configuração

É necessário configurar seu nome de usuario e email no git, para isso digite no terminal os seguintes comandos:

```bash
git config --global user.name "Seu usuario"
git config --global user.email "Seu email"
```

## Criando repositorio

Após ter criado uma conta no GitHub basta clicar no botão `` New `` no canto superior esquerdo para criar um novo repositorio.

![New](https://github.com/LevoratoJoao/GitHub-guide/assets/90461798/35dc379a-0397-4f6a-98b6-c73e4c1f606a)

GitHub vai mostrar várias opções, por hora vamos apenas colocar um nome para o repositorio e escolher se ele será publico ou privado.

![Criando_repositorio](https://github.com/LevoratoJoao/GitHub-guide/assets/90461798/570bd73e-183a-4666-b7ae-90ee8bed31ea)

Pronto, seu repositorio remoto esta criado :D

Mas ainda precisamos linkar ele a um repositorio local (no seu computador). O GitHub já nos mostra como fazer isso mostrando uma serie de comandos que devemos digitar no terminal.

![Linkando_repositorio](https://github.com/LevoratoJoao/GitHub-guide/assets/90461798/3093ec91-71b8-475c-837a-237a289c7300)

## Comandos basicos

Para criar um repositorio local, abra a pasta que deseja criar o repositorio no terminal e digite:

```bash
git init
```

Agora qualquer alteração que vocês fizer nos arquivos dessa pasta serão rastreados pelo git e você poderá mandar eles para o GitHub.

Para checar o status do seu repositorio, digite:

```bash
git status
```

Existem diversas maneiras de adicionar um arquivo ao seu repositorio, a mais simples é:

```bash
git add <nome_do_arquivo>
```

Caso queira adicionar todos os arquivos que foram modificados, digite:

```bash
git add .
```

Obs:
- O ponto representa todos os arquivos da pasta.
- `` git add * `` também adiciona todos os arquivos da pasta, porém ele não adiciona arquivos que começam com um ponto, como por exemplo `` .gitignore ``.

Para salvar as alterações feitas no repositorio, digite:

```bash
git commit -m "Mensagem do commit"
```

A mensagem do commit é uma mensagem que você escreve para descrever o que foi feito no commit, por exemplo: `` "Adicionado o arquivo tarefa.html" ``.

Para mandar este commit para o GitHub (repositorio remoto), digite:

```bash
git push origin main
```

Para pegar um repositorio remoto e clona-lo para o seu computador, digite:

```bash
git clone <link_do_repositorio>
```
<!-- add image about the link here -->

___
Estes são apenas os comandos basicos, existem muitos outros comandos que podem ser usados para facilitar o seu trabalho, para saber mais sobre eles, acesse a [documentação do git](https://git-scm.com/docs).

fique à vontade para contribuir com este guia :)

Links uteis:
- [Git com Bitbucket Cloud](https://www.atlassian.com/br/git/tutorials/learn-git-with-bitbucket-cloud)
