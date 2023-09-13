# Git e GitHub guide

Este repositorio é um guia inicial para quem quer aprender a usar Git e GitHub, nele você vai aprender comandos basicos para poder organizar seus projetos e trabalhos :)

<!--![GitHub_meme](https://github.com/LevoratoJoao/GitHub-guide/assets/90461798/b590945d-f8ea-4f78-b2e2-84740e607258)-->
<p align="center">
    <img width="400" src="Images/gitHub_meme.jpg" alt="GitHub Meme">
</p>

## Índice

* [O que é Git](#o-que-é-git)
* [Conhecendo GitHub](#conhecendo-github)
* [Instalando git](#instalação)
* [Criando um repositorio](#criando-um-repositorio)
* [Fazendo um commit](#fazendo-um-commit)


## O que é Git

Git é um sistema de controle de versão distribuído, usado principalmente no desenvolvimento de software, mas pode ser usado para registrar o histórico de edições de qualquer tipo de arquivo.

## Conhecendo GitHub

GitHub é uma plataforma de hospedagem de código-fonte com controle de versão usando o Git. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou Open Source de qualquer lugar do mundo.

Primeiro, crie uma conta no [GitHub](https://github.com/signup), se você ainda não tem uma.

## Instalação

### Windows

TODO

### Linux

Na maioria dos sistemas Linux o git já vem instalado, mas para verificarmos mesmo digite o seguinte comando no terminal:

```bash
git --version
```
<!-- IMAGEM DA VERSAO AQUI -->

Caso não apareça utilize o seguinte comando para fazer a instalação

```bash
sudo apt-get install git
```

## Configuração

É necessário configurar seu nome de usuario e email no git, para isso digite no terminal os seguintes comandos:

```bash
git config --global user.name "Seu usuario"
git config --global user.email "Seu email"
```

## Criando um repositorio

 Vamos começar criando um repositorio no GitHub

Após ter criado uma conta basta clicar no botão `` New `` no canto superior esquerdo para criar um novo repositorio.

![New](Images/new.png)

GitHub vai mostrar várias opções, por hora vamos apenas colocar um nome para o repositorio e escolher se ele será publico ou privado.

![Criando_repositorio](Images/criando_repositorio.png)

Pronto, seu repositorio remoto esta criado :D

Ainda precisamos linkar ele a um repositorio local (no seu computador). O GitHub já nos mostra como fazer isso mostrando uma serie de comandos que devemos digitar no terminal. Este é o comando para criar um repositorio local e ele deve ser feito dentro da pasta que deseja criar o repositorio:

```bash
git init
```

Vamos analisar os demais comandos no topico a seguir. Apos isso seu repositorio já está pronto para... <!-- ... -->

![Link_repositorio](Images/link_repositorio.png)

## Fazendo um commit

Agora qualquer alteração que vocês fizer nos arquivos dessa pasta serão rastreados pelo git e você poderá mandar eles para o GitHub.

Para checar o status do seu repositorio, digite:

```bash
git status
```

Existem diversas maneiras de adicionar um arquivo ao seu repositorio, a mais simples é:

```bash
git add .
```


Caso queira adicionar um arquivo que foi modificado em especifico, digite:

```bash
git add <nome_do_arquivo>
```

Obs:
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
