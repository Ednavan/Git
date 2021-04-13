# Git
Instalação do Github para sistemas


Acesse o site oficial e faça o download do instalador do GIT para Windows 
Depois de baixado, clique duas vezes no arquivo para iniciar o assistente de instalação. Basta seguir as instruções na tela, clicando em Next. Ao término, clique em Finish para concluir com êxito a instalação.

Abra o prompt de comando e digite os seguintes comandos no terminal:
git config --global user.name "João Silva"
git config --global user.email "exemplo@seuemail.com.br"


Instalação do Github no Liux(Ubuntu)
Abra o terminal e execute os seguintes comandos:
Sudo apt-get update 
Sudo apt-get install git

Verifique se a instalação ocorreu com sucesso usando git --version

Execute os seguintes comandos no terminal para configurar seu e-mail e nome de usuário que serão associados à sua conta GIT:
git config --global user.name "nome"
git config --global user.email "exemplo@seuemail.com.br


USANDO O GITHUB

Um repositório é o maior bem de qualquer projeto controlado por versão. Para transformar qualquer diretório em um repositório GIT, o simples comando git init <directory> pode ser utilizado. Uma pasta chamada .git também deve começar a existir no diretório em que o comando foi executado.

Por outro lado, se você já tem um diretório e deseja verificar (clone-lo), você pode usar o comando git clone. Se você estiver tentando verificar um repositório local, use o seguinte comando:

git clone /path/to/local/repository

Se você pretende verificar um repositório armazenado remotamente, use:

git clone user.name@host:/path/to/remote/repository










ERROS NO GITHUB

Faça um novo repo e envie o código existente novamente para o novo repo


git init não inicializa se você já tem uma pasta .git / em seu repositório. Então, para o seu caso, faça -

(1) rm -rf .git /

(2) git init

(3) git remote add origin  https: //repository.remote.url 652

(4) git commit -m “mensagem de confirmação”

(5) git push -f origin master

Observe que todas as configurações git, como repositórios remotos para este repositório, são limpas na etapa 1. Portanto, você deve configurar todas as URLs de repositório remoto novamente.

Além disso, tome cuidado com o -f na etapa 5: O remoto já tem alguma base de código com n commits, e você está tentando fazer todas essas mudanças em um único commit. Portanto, é necessário empurrar à força as alterações para remoto.
