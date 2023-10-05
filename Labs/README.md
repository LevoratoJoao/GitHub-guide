# Usando git nos laboratorios

## Índice

* [Criando um repositório](#criando-um-repositório)
* [Configurando o git](#configurando-o-git)
* [Fazendo um commit](#fazendo-um-commit)

## Criando um repositório

Após ter criado uma conta basta clicar no botão `` New `` no canto superior esquerdo para criar um novo repositório.

![New](../Images/new.png)

GitHub vai mostrar várias opções, por hora vamos apenas colocar um nome para o repositório, selecione a caixinha ``Add a README file ``, escolha se ele será publico ou privado e por fim Create repository.

![Criando_repositorio](../Images/criando_repositorio.png)

Agora que temos nosso repositório remoto criado vamos adiciona-lo na nossa home. Para isso, cline no botão ``Code`` e copie o link dele:

![Link_repositorio](../Images/clonar_repositorio.png)

Apos ter copiado o link do repositório abra o terminal na pasta HOME e digite o seguinte comando com o link:

```bash
git clone <link_do_repositório>
```
Pronto agora seu repositório do GitHub esta na sua Home, você pode fazer o mesmo processo de clonar o repositório na sua casa.

## Configurando o git
Para usar git nos laboratorios da UTF usando o Linux precisamos configurar usuario e email do git primeiro. 

Para fazer isso usamos os seguintes comandos:

```bash
git config --local user.name "Seu usuario"
git config --local user.email "Seu email"
```

Como os computadores dos laborátorios resetam sempre quando desligados precisamos fazer a configuração de forma local, por isso o comando recebe o `--local`, em sua casa este comando pode ser feito com `--global`.

## Fazendo um commit
Agora qualquer alteração que vocês fizerem nos arquivos dessa pasta do repositório serão rastreados pelo git e você poderá mandar eles para o GitHub.

Para checar o status do seu repositório, digite:

```bash
git status
```

Existem diversas maneiras de adicionar um arquivo ao seu repositório, a mais simples é:

```bash
git add .
```

Caso queira adicionar um arquivo que foi modificado em especifico, digite:

```bash
git add <nome_do_arquivo>
```

Obs:
- `` git add * `` também adiciona todos os arquivos da pasta, porém ele não adiciona arquivos que começam com um ponto, como por exemplo `` .gitignore ``.

Para salvar as alterações feitas no repositório, digite:

```bash
git commit -m "Mensagem do commit"
```

A mensagem do commit é uma mensagem que você escreve para descrever o que foi feito no commit, por exemplo: `"Adicionado o arquivo tarefa.html"`.

Para mandar este commit para o GitHub (repositório remoto), digite:

```bash
git push origin main
```

Apos isso o git vai solicitar um login no terminal, digite seu usuario do GitHub e após isso ele irá pedir a senha, porém, não é a mesma senha do GitHub mas sim um token de acesso. Vamos criar um:

Na página do GitHub clique no seu perfil no canto superior esquerdo da página e vá em `Settings`

![settings](/Labs/Images/settings.png)

Na página de configurações na parte esquerda, navegue até encontrar a opção `Developer settings`.

![developer_settings](/Labs/Images/developer_settings.png)

Agora acesse `Tokens (classic)`

![token_classic](/Labs/Images/token_classic.png)

![generate_new_toke](/Labs/Images/generate_new_token.png)

Temos uma serie de opções para o token, coloque um nome para ele, selecione o tempo de expiração e selecione a opção `repo`

![token_options](/Labs/Images/token_options.png)

Clique no botão `Generate token` no final da página. Copie esse token e salve em um arquivo txt para não perdê-lo, se você perder este token terá que criar um novo.

```bash
git pull
```

git pull é um comando que irá puxar as alterações do repositório remoto que não estão no repositório local, sempre que fizer alterações em sua casa use este comando para atualizar a pasta nos laboratórios.

___
Estes são apenas os comandos basicos, existem muitos outros comandos que podem ser usados para facilitar o seu trabalho, para saber mais sobre eles, acesse a [documentação do git](https://git-scm.com/docs).

Links uteis:
- [Git com Bitbucket Cloud](https://www.atlassian.com/br/git/tutorials/learn-git-with-bitbucket-cloud)