#Sobre GitHub
##Do GitHub
- Git init - inicia o git dentro de uma pasta
- git add * - selecionar os arquivos para dar commit
- git commit -m “escrever uma mensagem” - comando para dar commit no repositorio local
- git remote add origin link -  para selecionar os arquivos e mostrar o caminho que devem ir
- git push origin master - para de fato dar commit e colocar os arquivos no repositorio remoto
- git pull oring master - puxa os arquivos do remoto para o local
- git clone link - clonar um repositorio
- git config —global [user.email](http://user.email) or [user.name](http://user.name) - configurar o nome e email do github
- git config —global unset [user.email](http://user.email) or [user.name](http://user.name) - apaga o nome ou email para rescrever

##Do prompt 
- Dir - Lista as pastas dentro de um diretorio
    - Dir -a
- Cd - Change direct, mudar o diretorio que esta
- Mkdir - Cria uma pasta
- Echo - Serve para duas coisas:
    - Printar na tela algo
    - Criar um arquivo → echo hello > hello.txt
        - Criando um arquivo de texto e dentro dele tem escrito hello
- Del - Serve apenas para deletar arquivos
- Rmdir - Serve para deletar as pastas

##Estrutura
- Untrecked - arquivos desconhecidos para o github, ao usar o add vai para stage
- Tracked - Arquivos que o github conhece
    - Unmodified - Arquivos que não tem nenhuma mudança, ao modificar vai para modified
    - Modified - Arquivos com mundaças mas não prontos para commit, ao dar add vai para staged
    - Staged - Pronto para “commitar”
 ##Informações
 - Sha1 - Secure hash algorthm, embaralha as informações criando um codigo de 40 digitos
- Estrutura basica: Todos tem o sha1 se alguma informação mudar vai mudar o sha1
    - Blobs - Armazena os metadados, como tamanho tipo
    - Trees - Armazenas os blobs e os nomes dos arquivos, alem de apontas para os blobs e outras trees
    - Commit - Armazena todos ou outros alem do timestamp
- Chave ssh - Uma chave que mostrar ao GitHub que é seguro o pc
    - ssh-keygen -t ed25519 -c email
    - cat nome
    - eval$(ssh-agent * -s)