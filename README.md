# Curso - Frontend
#### EBAC

## GIT
___
### Conceitos de versionamento

  - Histórico
  - Controle de versão
  - Quem alterou
  - O quê alterou
  - Quando alterou
  - Todos os arquivos
  - Evolução continua

Arquivo A | Versão 1 | Versão 2<br>
Arquivo B | Versão 1 | Versão 2

___
### Instalação do Git

https://git-scm.com/

  - Windows: https://git-scm.com/download/win
  - Linux: (apt-get): sudo apt-get install git
  - Mac: (brew): brew install git

___
### Criar conta no GitHub

___
### Clonar projeto e outros comandos

  - `git clone https://github.com/andersonmace/curso-frontend-ebac.git`
  - `git status`
  - `git add *` (pega todos os arquivos)
  - `git config --global user.name "Anderson Macedo"`
  - `git config --global user.email andersonmac@gmail.com`
  - `git commit -m "Texto da alteração"`
  - `git push` (Enviar arquivos)
  - `git pull` (Receber arquivos)
  - `git branch`

___
### Commits

**`git commit -m "Texto da alteracao"`**

Informação de alterção
  - após testado todo o seu código

___
### Branches

**`git branch`** São as ramificações do código / versões paralelas.

  - main / master (branch principal, vai para produção, quando o projeto é publicado).
  - develop (uma branch criada para desenvolvimento do código antes de ser enviada para branch principal).
    - DOD (Definition of Done) são critérios de aceite para o projeto ser publicado na main branch.
    - Exemplo: **`git checkout -b dev`** (faz o checkout da branch atual e cria uma nova com nome "dev" e faz uma cópia dos arquivos nela).
    - Após comitar e finalizar todas alterações na brach atual, pode-se fazer o **`git fetch --all`** para verificar se há mudanças no projeto remoto.
    - **`git push --set-upstream origin dev`**: serve para dar push em uma branch nova, no caso a branch 'dev'.
    - **`git checkout main`**: muda da branch atual para branch main.

  - versionamento 0.1.x (versão beta, em desenvolvimento / alterações finais feitas nessa versão / correção de bugs)
  - versionamento 0.2.11
  - versionamento 1.0.0 (versão pronta para publicação e colocada na main brach)

___
### Merge

**`git merge main`**
 - Mescla de branches (Após finalizar e publicar os arquivos na branch 'dev', é hora de mesclar para branch principal 'main').
 - Você pode precisar resolver conflitos manualmente

___
### Pull Requests

**`git pull`**
 - Mescla de branches no repositório
 - Permite o code review
 - O repositório resolve os conflitos automaticamente

___
### GitFlow

**`git flow init`**
 - Fluxo do Git ()

**`git flow feature start nome-da-feature`**
 - Inicia uma nova feature branch feature/nome-da-feature

**`git flow feature finish nome-da-feature`**
 - Finaliza a branch feature/nome-da-feature

___
### Git Ignore

**`touch .gitignore`**
 - Adiciona um arquivo que ignora outros arquivos a irem pra branch
 - Exemplo: "*.zip" - evita subir qualquer arquivo .zip para a branch
 - Lembrar de colocar **`git add .gitignore`**
