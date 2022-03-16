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
  - git clone https://github.com/andersonmace/curso-frontend-ebac.git
  - git status
  - git add * (pega todos os arquivos)
  - git config --global user.name "Anderson Macedo"
  - git config --global user.email andersonmac@gmail.com
  - git commit -m "Texto da alteração"
  - git push (Enviar arquivos)
  - git pull (Receber arquivos)
  - git branch

___
### Commits
**git commit -m "Texto da alteracao"**

Informação de alterção
  - após testado todo o seu código

___
### GitFlow
Fluxo do Git

___
### Branches
**git branch** São as ramificações do código / versões paralelas

  - main / master (branch principal, vai para produção, quando o projeto é publicado)
  - develop (uma branch criada para desenvolvimento do código antes de ser enviada para branch principal)
    - DOD (Definition of Done) são critérios de aceite para o projeto ser publicado na main branch.
    - Exemplo: **git checkout -b dev** (faz o checkout da branch atual e cria uma nova com nome "dev" e faz uma cópia dos arquivos nela)

  - versionamento 0.1.x (versão beta, em desenvolvimento / alterações finais feitas nessa versão / correção de bugs)
  - versionamento 0.2.11
  - versionamento 1.0.0 (versão pronta para publicação e colocada na main brach)