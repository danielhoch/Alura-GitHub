# Alura-GitHub
## Cursos / Treinamentos de Git e GitHub

Comando executados.

#### Verificar a versão do Git instalada
git --version

# Iniciando um repositório do git
.git init

# Mostra o status dos arquivos
git status

# Monitora todos os arquivos da pasta atual
git add .

# Monitora um arquivo específico, adicionando para commit
git add index.html

# Rollback nas alterações dos arquivos que não foram marcadas para commit
git checkout -- nome do arquivo

# Commit de um arquivo ou projeto. commit / -m -> Mensagem do commit
git commit -m "Criando arquivo index.html com lista de cursos"

# Rollback nos nos arquivo que foram marcados para commit. O arquivo continua com as alterações
git reset HEAD nome do arquivo

# Desfazendo um commit
git log
git revert 0e58a0a007067a7e036d1f17ba9011f8cd81f907 (valor do commit hash)

# Verificando históricos de commits
git log

# Listar commits em linhas reduzidas
git log --oneline

# Exibir linhas alteradas com detalhes
git log -p

# Exibir apenas os dois últimos commits
git log -n 2

# Alterando configurações do git na pasta local
git config --local user.name "Daniel Herbert Hoch"

# Verificando o nome
git config user.name

# Verificando o email
git config user.email

# Adicionado arquivo .gitignore. Todo conteúdo dentro do arquivo .gitignore como pastas e arquivos, serão desprezados pelo git no momento #do push.
git add .gitignore

# Commit do arquivo
git commit -m "adicionando .gitignore"

# Listando repositorio remoto
git remote

# Listando o diretório do repositório remoto e local
git remote -v

# Adicionando um repositório origin do gitHub
git remote add origin https://github.com/danielhoch/Alura-GitHub.git

# Baixando um repositorio do gitHub
git clone https://github.com/danielhoch/Alura-GitHub.git

# Enviando os dados do repositório origin do gitHub
git push origin master

# Criando branch
git branch titulo

# Criando branch com atalho. b -> Branch
git checkout -b lista

# Alterar de branch
git checkout titulo

# Comparando dois commits. O código do commit de hash pode ser utilizado apenas com 7 digitos.
git log --oneline
git diff 59d9688..81d1d81

# Gerando versão (Tag)
git tag -a v12.1.28 -m "Lançando a primeira versão (BETA)"

**Enviando versão 12.1.28 para o servidor remoto**
# Atualizando servidor
git push origin master

# Enviando a tag 12.1.28
git push origin v12.1.28
