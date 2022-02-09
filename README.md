<h1 align="center">
📄<br>Padrões de commits - Prometeon BR
</h1>

<h1 align="center">
  <img src="gitcommit.png">
</h1>

<p>
  Este repositório foi criado com base no repositório do user <a href="https://github.com/iuricode">@iuricode</a> e busca padronizar o commits e o sugerir um workflow aos colaboradores que utilizam as ferramentas Git e Github dentro da empresa.
</p>

## ⌨️ Tipo e Descrição

O commit semântico possui os elementos estruturais abaixo (tipos), que informam a intenção do seu commit ao utilizador(a) de seu código.

- `fix` - Commits do tipo fix indicam que seu trecho de código commitado está solucionando um problema (bug fix), (se relaciona com o PATCH do versionamento semântico).

- `feat`- Commits do tipo feat indicam que seu trecho de código está incluindo um novo recurso (se relaciona com o MINOR do versionamento semântico).

- `docs` - Commits do tipo docs indicam que houveram mudanças na documentação, como por exemplo no Readme do seu repositório. (Não inclui alterações em código).

- `style` - Commits do tipo style indicam que houveram alterações referentes a formatações de código, semicolons, trailing spaces, lint... (Não inclui alterações em código).

- `refactor` - Commits do tipo refactor referem-se a mudanças devido a refatorações que não alterem sua funcionalidade, como por exemplo, uma alteração no formato como é processada determinada parte da tela, mas que manteve a mesma funcionalidade, ou melhorias de performance devido a um code review.

- `build` - Commits do tipo build são utilizados quando são realizadas modificações em arquivos de build e dependências.

- `test` - Commits do tipo test são utilizados quando são realizadas alterações em testes, seja criando, alterando ou excluindo testes unitários. (Não inclui alterações em código)

- `chore` - Commits do tipo chore indicam atualizações de tarefas de build, configurações de administrador, pacotes... como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em código)

## 🌗 Estágio

- `partial` - Commits do tipo partial são utilizados quando são realizadas alterações parciais dentro da branch utilizada que ja carregam uma quantidade relevante de modificações.

- `final` - Commits do tipo final indicam que a issue ja foi completamente resolvida e que esta é a versão final para ser realizada um merge junto à branch _master_.

## 🪜 Passo a passo

<p>
  Após a abertura da issue pelo admin do projeto, em seu ambiente de trabalho seguir os seguintes comandos (exemplo campo novo no app):
</p>

- Acessar a branch principal do repositório (geralmente **master** ou **main**) e importar os dados mais recentes do repositório remoto:

```bash
git checkout master
git pull master
```

- Em seguida criar uma nova branch com o tipo de tarefa a ser realizada e o nome da tarefa:

```bash
git checkout -b feat/campo-novo
```

- Apos concluir a tarefa ou a etapa, adicionar os arquivos editados para a staging area:

```bash
git add . # para adicionar todos os arquivos editados
git add arquivo.py # para adicionar somente o arquivo desejado
```

- Realizar um 'save' das edições armazenadas no staging area através do git commit **atendendo aos padrões de commits** e realizar um push no repositório remoto:

```bash
git commit -m 'feat (campo-novo): ref issue #93 - final'
git push
```

## 💻 Pull Request

- Após realizar o push no repositório remoto, solicitar um pull request dentro do Github selecionando a branch principal e a branch referente a issue solucionada e aguardar a aprovação do admin do projeto.

<br>[⬆ Voltar ao top](#padrões-de-commits-) <br>
