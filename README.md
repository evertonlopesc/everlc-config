Setting Ubuntu 20.04
======================

### Passo a passo como estou configurando minha máquina.

Instalar as principais ferramentas;
-----------------------------------
~~~bash
sudo apt install -y git curl wget zsh neovim tilix libncurses5-dev
~~~

_______________________________________________________________

GIT
-----------------

Verifique se esse arquivo está criado: **.gitconfig**, caso contrário crie e cole esses alias dentro
~~~bash
[user]
	name = Seu Nome
	email = seu@email
[core]
	editor = vim
[color]
	status = auto
	branch = auto
	interactive = auto
	diff = auto
[alias]
	st = status
	co = checkout
	br = branch
	ci = commit
	cm = "commit -m"
	all = "add -A"
	restaged = "restore --staged"
	last = "log -1 HEAD"
	logone = "log --oneline"
	slog = "log --oneline --graph"
~~~

**No exemplo abaixo eles executam o mesmo comando**
~~~bash 
git status && git st
~~~

_______________________________________________________________________________________________________________________________________________________

ZSH, ZINIT e OH-MY-ZSH
----------------------

Executar esse comando abaixo
~~~bash 
chsh -s $(which zsh)
~~~

*Fecha o terminal e abre novamente.*

Instalar o oh-my-zsh

[Site guia do ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)

Usando o editor de sua escolha, abra o arquivo **.zshrc** descomenta o alias do **zshconfig** e addiciona os plugins que você quiser e escolha o tema.
~~~bash
vim ~/.zshrc
~~~

> **antes ->** # alias zshconfig="mate ~/.zshrc" **| depois ->** alias zshconfig="vim ~/.zshrc"

Plugins para o zsh: [Guia Zinit plugins](https://github.com/zdharma/zinit)

Adicionar no final do arquivo **.zshrc** os seguintes comandos:
~~~bash
zinit load zdharma/history-search-multi-word
zinit light zsh-users/zsh-autosuggestions
zinit light zdharma/fast-syntax-highlighting
zinit snippet https://gist.githubusercontent.com/hightemp/5071909/raw/
~~~

Crie seu tema ZSH: [Customer ZSH](https://blog.carbonfive.com/writing-zsh-themes-a-quickref/)

_______________________________________________________________________________________________

Estilizando o ambiente linux
----------------------------

[Flat Remix](https://www.osradar.com/install-flat-remix-theme-ubuntu/)

_______________________________________________________________________

Google Chrome
-------------------------

[Site guia de instalação](https://pt.wikihow.com/Instalar-o-Google-Chrome-Usando-o-Terminal-no-Linux;)

______________________________________________________________________________________________________

Micrsoft-Edge
--------------------------

[Site oficial](https://www.microsoftedgeinsider.com/pt-br/download?platform=linux-deb)

_______________________________________________________________________________________

SNAP
----

Executar o comando
~~~bash
sudo apt install snap
~~~

VS Code via SNAP, gosto dessa versão
~~~bash
sudo snap install code --classic
~~~

_____________________________________

Dependências para Desenvolvimento
---------------------------------

Executar o comando
~~~bash
sudo apt -y install build-essential gnupg2 autoconf m4 libncurses5-dev libwxgtk3.0-gtk3-dev libgl1-mesa-dev libglu1-mesa-dev libpq-dev libpng-dev libssh-dev unixodbc-dev xsltproc fop libxml2-utils libncurses-dev openjdk-11-jdk default-jdk libssl-dev exuberant-ctags ncurses-term silversearcher-ag fontconfig imagemagick libmagickwand-dev libreadline-dev vim-gtk3 gcc g++
~~~

________________________________________________________________________________________________________________________________________________________________

RVM -> Gerênciar versão do Ruby
-------------------------------
Install GPG2 keys. *Chave atualizada*
~~~bash
gpg2 --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
~~~

[How To Install Ruby On Rails On Ubuntu 20.04 - itzgeek](https://www.itzgeek.com/post/how-to-install-ruby-on-rails-on-ubuntu-20-04/)

_____________________________________________________________________________________________________________________________________
PostgreSQL
----------

[How to Install PostgreSQL and pgAdmin4 in Ubuntu 20.04 - TecAdmin](https://tecadmin.net/how-to-install-postgresql-in-ubuntu-20-04/)

[Para analisar depois](https://computingforgeeks.com/install-postgresql-12-on-ubuntu/) *Não testado* | 
[Para analisar depois](https://linuxize.com/post/how-to-install-postgresql-on-ubuntu-20-04/) *Não testado* | 
[Para analisar depois](https://www.howtodojo.com/install-postgresql-13-ubuntu-20-04/) *Não testado* | 

______________________________________________________________________________________________________________________________________

SSH
---

[Referência sobre os tipos de chaves](https://goteleport.com/blog/comparing-ssh-keys/)

[Gerar chave SSH RSA - Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04-pt)

[Gerar chave ed25519](https://blog.peterruppel.de/ed25519-for-ssh/)

[Install OpenSSH Server](https://ubuntu.com/server/docs/service-openssh)

____________________________________________________________________________________________________________________________________
