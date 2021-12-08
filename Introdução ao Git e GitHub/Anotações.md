# Areas do git por baixo dos panos

 - Untracked - area que esta fora do tracked, que seria a area fora do repositorio, todos os outros estão dentro do Tracked
ao usar git add, ira jogar do untracked ao staged.

 - Unmodifed - partes do codigo sem alteração, irão pro modified ao editar o arquivo.

 - Modified - Modificações no codigo, que ira para o Staged.

 - Staged - 'Preparação dos bastidores' preparação para fazer o commit, que ira fazer ir para o unmodified.

# Comandos do Git

## Configuração do git
Nome: config --global user.name "Name"

Email: config --global user.email email@hotmail.com

Editor: git config --global core.editor vim

Ferramenta de merge: git config --global merge.tool vimdiff

Gitignore: git config --global core.excludesfile ~/.gitignore

Listar configurações: git config --list

## Repositório Local
Criar repositório: git init

Verificar estado: git status

### Adicionar arquivo/diretorio(staged area)

Arquivo: git add arquivo.txt

Diretorio: git add diretorio

Tudo: git add . Ou git add *

gitignore: git add -f arquivo_no_gitignore.txt

### Comitar
Comitar arquivo: git commit arquivo

Comitar varios arquivos: git commit arquivo.txt segundoarquivo.txt

Comitar com mensagem: git commit arquivo.txt -m "minha mensagem de commit"

### Remover
Arquivo: git rm arquivo.txt

Diretorio: git rm -r diretorio

## Repositorio Remoto

Exibir diretorios remotos: git remote, git remote -v

Vincular local ao remoto: git remote add origin git@github.com:localdorepositorioremoto

Enviar arquivos/diretorios ao repositório remoto: git push -u origin master

### Atualizar repositório local de acordo com o repositório remoto
Atualizar o local com do remoto: git pull

Buscar informações mas nao aplica-las: git fetch

### Clonar
Clonar o repositório: git clone git@github.com:oendereço

Link para mais informações dos comandos: https://gist.github.com/leocomelli/2545add34e4fec21ec16
