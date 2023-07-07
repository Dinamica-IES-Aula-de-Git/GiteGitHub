## Criando um Repositório Remoto no GitHub e Clonando com o Git Clone
1. Acesse o site do GitHub (github.com) e faça login na sua conta.
2. Clique no botão `"New"` ou `"Novo"` para criar um novo **repositório**.
3. Preencha o nome do repositório, descrição (opcional) e escolha as opções de visibilidade.
4. Clique em `"Create repository"` ou `"Criar repositório"` para criar o repositório no GitHub.
5. Após a criação do repositório, você verá o endereço HTTPS ou SSH do repositório.
6. No terminal, navegue até a pasta onde deseja clonar o repositório usando o comando `cd <caminho-da-pasta>`.
7. Execute o comando `git clone <endereço-do-repositório>` para clonar o repositório remoto para o seu computador.
8. Aguarde até que o processo de clonagem seja concluído.  
  Será mostrada uma mensagem semelhante a esta:
```
  Cloning into 'nome-do-repositorio'...
  remote: Enumerating objects: 100, done.
  remote: Counting objects: 100% (100/100), done.
  remote: Compressing objects: 100% (80/80), done.
  remote: Total 100 (delta 20), reused 0 (delta 0), pack-reused 0
  Receiving objects: 100% (100/100), 10.15 KiB | 2.54 MiB/s, done.
  Resolving deltas: 100% (20/20), done.
```

  
Agora você tem uma cópia local do repositório remoto no seu computador.  
Você pode começar a trabalhar no repositório local, fazer alterações, commits e push para o repositório remoto conforme necessário.  

Para adicionar arquivo ou modificações, faça:  
10. Crie ou adicione arquivos para dentro da pasta do repositório clonado na sua máquina.  
11. Abra o Git Bash, e navegue até o local da pasta utilizando os comandos `cd <caminho-da-pasta>`.  
12. Execute o comando `git status` para saber se há novas alterações, se houver será exibido uma mensagem semelhante a esta:
```
  On branch main
  Your branch is up to date with 'origin/main'.
  
  Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
          modified:   arquivo1.txt
          modified:   arquivo2.cpp
  Untracked files:
    (use "git add <file>..." to include in what will be committed)
          novo_arquivo.txt
  
  no changes added to commit (use "git add" and/or "git commit -a")

```

  
13. Execute o comando `git add .`, para adicionar todas as alterações feitas nos arquivos do seu repositório local.
14. Execute o comando `git commit -m "Mensagem"`, para registrar as alterações feitas nos arquivos que foram previamente adicionados ao índice (staging area) com o comando "git add".
15. E por fim, execute o comando `git push origin main` enviando as alterações para o seu repositório remoto.
  
Para trazer as alterações feitas no repositório remoto para o seu repositório local e alterar o novo arquivo atualizado, siga o seguinte passo.  
16. Execute o comando `git pull origin main`, para trazer os arquivos atualizados, na qual será exibida a seguinte mensagem:
```
   Updating bf262a2..ff3db8b
   Fast-forward
   arquivo.txt | 5 +++++
   1 file changed, 5 insertions(+)
```

  
Pronto, agora você poderá fazer alterações e enviar para o repositório local e remoto.
