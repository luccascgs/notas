# Inicializando GIT local #

## Primeiro confira se o git está instalado ##

``bash
git --version``

## Entre na pasta documentos ##

``bash
cd Documents/``

## Configure o nome de usuário ##

``bash
git config --global user.name "'nome'"``

## Configure o e-mail ##

``bash
git config --global user.email "'email'" ``

## Crie a pasta ##

mkdir "nome da pasta"

# Configurando o GitHub #

Verificar se existe chave

``bash
ssh.ls -al ~/.ssh
``
## Adicionar uma nova chave ##

``bash
(ID)ssh-keygen -t ed25519 -C "your_email@example.com"
``

## Inicializar agente-ssh ##

``bash
eval "$(ssh-agent -s)"
``

## Copiar chave ssh.##

``bash
clip < ~/.ssh/id_ed25519.pub
``

## Adicionar Chave ##

Github -> Settings -> SSH and GPG keys -> New SSH key -> Colar

## Testar Conexão ##

``bash
ssh -T git@github.comyes
``

## Adicionar chave ssh ao agente ##

``bash
ssh-add ~/.ssh/id_ed25519
``