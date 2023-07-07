## O que é uma chave SSH?
Uma chave SSH é um par de chaves criptográficas composto por uma chave pública e uma chave privada. Ela oferece um método de autenticação seguro ao estabelecer conexões criptografadas entre um cliente e um servidor. Ao criar uma chave SSH, você obtém os seguintes benefícios:
  
* **Segurança:** As chaves SSH usam criptografia forte para garantir a segurança das conexões.  
* **Autenticação simplificada:** Com uma chave SSH configurada, você não precisa digitar sua senha toda vez que interage com o servidor remoto.  
* **Conveniência:** A autenticação SSH é mais rápida e eficiente do que inserir repetidamente suas credenciais.  
* **Uso em várias plataformas:** Uma chave SSH pode ser usada em diferentes serviços que suportam autenticação SSH.  
  
No contexto do Git e GitHub, criar uma chave SSH permite que você se conecte e autentique em seu repositório remoto sem a necessidade de inserir suas credenciais a cada operação. Isso torna o processo de colaboração mais seguro, eficiente e conveniente.

  
## Como fazer uma chave SSH
1. No terminal execute o comando: `ssh-keygen -t rsa -b 4096 -C "seu-email@example.com"`. Substitua `"seu-email@example.com"` pelo seu endereço de e-mail associado à sua conta do GitHub.
  
2. Em seguida, ele solicitará um local para salvar a chave. Por padrão, ele irá sugerir o caminho `C:\Users\<seu-usuário>\.ssh\id_rsa`, onde `<seu-usuário>` é o nome de usuário do seu sistema Windows.
  
3. Você pode pressionar Enter para aceitar o local padrão ou especificar um caminho personalizado, se preferir.
  
4. Ele também solicitará uma senha para proteger a chave privada. Você pode optar por definir uma senha ou deixar em branco pressionando Enter (mais adequado).
  
Após a geração da chave, ela será salva no local especificado. Agora você pode adicionar a chave pública ao seu perfil do GitHub para usá-la como forma de autenticação. Aqui está um passo a passo de como fazer isso:

1. Copie a chave pública para a área de transferência:  
1.1. No terminal, execute o comando `cat ~/.ssh/id_rsa.pub` para exibir a chave pública.  
1.2. Selecione e copie a chave completa que é exibida no terminal.  

2. Acesse o GitHub e faça login na sua conta.

3. No canto superior direito, clique na sua foto de perfil e selecione `"Settings"` uo `Configurações` no menu suspenso.

4. Na página "Settings", clique em `"SSH and GPG keys"` ou `Chaves SSH e GPG` no menu lateral.

5. Clique no botão `"New SSH key"` ou `Nova chave SSH`.

6. Em `"Title"` ou `Título`, dê um nome descritivo para a chave, como `"Meu Computador Pessoal"`.

7. Na caixa `"Key"` ou `Chave`, cole a chave pública que você copiou anteriormente.

8. Clique em `"Add SSH key"` ou `Adicionar chave SSH` para salvar a chave.  
  
Agora a sua chave SSH está adicionada ao seu perfil do GitHub. Isso permitirá que você se autentique nos repositórios do GitHub usando a chave SSH ao invés de inserir suas credenciais (usuário e senha) a cada interação.

