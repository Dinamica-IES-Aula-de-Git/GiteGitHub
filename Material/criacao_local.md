## Criando um Repositório Local com o Git Init
1. Abra o terminal ou o Git Bash no seu computador.
2. Navegue até a pasta onde deseja criar o repositório usando o comando `cd` `<caminho-da-pasta>`.
3. Execute o comando `git init` para **inicializar um novo repositório local**.
4. Agora você tem um repositório Git vazio na pasta selecionada.
5. Adicione arquivos ao repositório criando-os ou copiando-os para a pasta do repositório.
6. Verifique o status dos arquivos usando o comando `git status`.
   Se houver alterações pendentes para ser levadas ao repositório local, irá ser exibida uma mensagem semelhante a esta:
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
  
8. Utilize o comando `git add` `<nome-do-arquivo>` para adicionar os arquivos ao controle de versão do Git.
9. Faça um commit das alterações usando o comando `git commit -m "Mensagem do commit"`.
  
Agora você precisa conectar o repositório local a um repositório remoto no GitHub ou em outra plataforma, seguindo as etapas adequadas.  
10. Vá até seu remositório do GitHub e copie o link ssh.  
11. Execute o comando `git remote add origin git@github.com:<seu-nome-de-usuario>/<seu-repositorio>.git`, substituindo `<git@github.com:<seu-nome-de-usuario>/<seu-repositorio>.git>` pelo link.  
12. Agora o repositório local está conectado ao repositório remoto usando a chave SSH.  
13. Para enviar seus arquivos do repositório local ao repositório remoto do GitHub, execute o comando `git push origin main`. Será exibida uma mensagem semelhante a esta:  
```
    Enumerating objects: 5, done.
    Counting objects: 100% (5/5), done.
    Delta compression using up to 4 threads
    Compressing objects: 100% (3/3), done.
    Writing objects: 100% (3/3), 300 bytes | 100.00 KiB/s, done.
    Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
    To git@github.com:<seu-nome-de-usuario>/<seu-repositorio>.git
       1234567..890abc1  main -> main
```
    
Agora você tem um repositório local configurado e pode continuar trabalhando nele, fazendo alterações, commits e push para o repositório remoto, se aplicável.
