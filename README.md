# Principais comandos que serão usados na Dinâmica.

## Configurando chave SSH:

* `ssh keygen -t rsa -b 4096 -C "seu-email@example.com"`
* `cat ~/.ssh/id_rsa.pub`

## Configurando seu Git:

* `git config --global user.name "Seu Nome"`
* `git config --global user.email seu-email@example.com`

## Clonando o repositório:

* `git clone link_SSH_do_repositorio`

## Verificando alterações e fazendo o commit:

* `git status`
* `git add .`
* `git commit -m "Título do commit"`
* `git log`

## Fazendo o push pro Github:

* `git branch -M main`
* `git push origin main`
