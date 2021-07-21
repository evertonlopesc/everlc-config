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

Instalar o oh-my-zsh ([Site oficial](https://github.com/ohmyzsh/ohmyzsh))
~~~bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
~~~

Usando o editor de sua escolha, abra o arquivo **.zshrc** descomenta o alias do **zshconfig** e addiciona os plugins que você quiser e escolha o tema.
~~~bash
vim ~/.zshrc
~~~

> **antes ->** # alias zshconfig="mate ~/.zshrc" **| depois ->** alias zshconfig="vim ~/.zshrc"

Adicionar os plugins
~~~bash
plugins=(
  git
  bundler
  dotenv
  osx
  rake
  rbenv
  ruby
  gem
  postgres
  rails
)
~~~

Plugins para o zsh: [Guia Zinit plugins](https://github.com/zdharma/zinit)

~~~bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/zdharma/zinit/master/doc/install.sh)"
~~~

Adicionar no final do arquivo **.zshrc** os seguintes comandos:
~~~bash
zinit load zdharma/history-search-multi-word
zinit light zsh-users/zsh-autosuggestions
zinit light zdharma/fast-syntax-highlighting
zinit snippet https://gist.githubusercontent.com/hightemp/5071909/raw/
~~~

Crie seu tema ZSH: [Customer ZSH](https://blog.carbonfive.com/writing-zsh-themes-a-quickref/)

Fechar e abrir o terminal, depois
~~~bash
sudo apt update
~~~

Precisa reiniciar o sistema
~~~bash
reboot
~~~

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

Configuração VS Code. Hoje eu trabalho com Ruby on Rails, logo essa conf. está direcionada a ele.
~~~json
{
	"editor.fontFamily": "'CaskaydiaCove Nerd Font'",
	"editor.fontSize": 14,
	"editor.wordWrapColumn": 80,
	"editor.wordWrap": "wordWrapColumn",
	"editor.autoIndent": "full",
	"editor.insertSpaces": true,
	"editor.minimap.enabled": false,
	"editor.cursorStyle": "line",
	"editor.cursorBlinking": "expand",
	
	"cSpell.language": "en,pt,pt_BR",

	"files.trimTrailingWhitespace": true,
	"files.autoSaveDelay": 5000,

	"explorer.openEditors.visible": 0,

	// CUSTOM VS CODE
	"workbench.colorTheme": "One Monokai",
	"workbench.iconTheme": "vscode-icons",
	"workbench.activityBar.visible": true,
	"workbench.colorCustomizations": {
		"editor.background": "#000000",
		"sideBar.background": "#000000",
		"sideBar.border": "#ffffff",
		"activityBar.background": "#550000",
		"activityBar.activeBorder": "#ffffff",
		"activityBar.activeFocusBorder": "#ffffff",
		"activityBar.border": "#ffffff",
		"activityBar.foreground": "#ffffff",
		"activityBar.inactiveForeground": "#000000",
		"statusBar.foreground": "#ffffff",
		"statusBar.background": "#550000",
		"statusBar.border": "#ffffff",
		"tab.activeBackground": "#000000",
		"tab.activeForeground": "#ffffff",
		"tab.inactiveBackground": "#333333",
		"tab.inactiveForeground": "#555555",
		"tab.activeBorder": "#ff0000",
	},

	"[css]": {
		"editor.suggest.insertMode": "replace",
		"editor.tabSize": 2
	},

	"[ruby]": {
		"editor.tabSize": 2,
	},

	"emmet.includeLanguages": {
		"ruby":  "html",
		"erb": "html",
	},

	"solargraph.autoformat": true,
	"solargraph.diagnostics": true,
	"solargraph.formatting": true,
	"solargraph.completion": true,
	"solargraph.symbols": true,
	"solargraph.references": true,

}
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

Create the file repository configuration:
~~~ bash
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'
~~~

Import the repository signing key:
~~~ bash
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
~~~

Update the package lists:
~~~ bash
sudo apt-get update
~~~

Modifique o arquivo: 
~~~ bash
sudo vim /etc/apt/sources.list.d/pgdg.list
~~~

Acrescentar [arch=amd64] nesse arquivo, conforme código abaixo:
> deb [arch=amd64] http://apt.postgresql.org/pub/repos/apt/ focal-pgdg main

Instalar o PostgreSQL:
~~~ bash
sudo apt-get -y install postgresql-13 postgresql-contrib-13 postgresql-server-dev-13
~~~

Execute:
~~~ bash
pg_ctlcluster 13 main start
~~~

Caso o de cima dê erro, execute:
~~~ bash
sudo systemctl start postgresql@13-main
~~~
Siga o apartir do passo 2:

[Como instalar o PostgreSQL no Ubuntu 20.04](https://www.digitalocean.com/community/tutorials/how-to-install-postgresql-on-ubuntu-20-04-quickstart-pt)

Criar usuário com senha:
~~~ bash
psql
~~~

Comando para criar usuário com senha:
~~~ bash
CREATE USER <name_user> WITH PASSWORD '<password>';
~~~

Verificar usuário no banco:
~~~ bash
\du
~~~

Criando o banco de dados pertencente a um usuário:
~~~ bash
CREATE DATABASE <name_database> OWNER <user_name>;
~~~

Verificar banco de dados:
~~~ bash
\l
~~~

______________________________________________________________________________________________________________________________________

SSH
---

[Referência sobre os tipos de chaves](https://goteleport.com/blog/comparing-ssh-keys/)

[Gerar chave SSH RSA - Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04-pt)

[Gerar chave ed25519](https://blog.peterruppel.de/ed25519-for-ssh/)

[Install OpenSSH Server](https://ubuntu.com/server/docs/service-openssh)

____________________________________________________________________________________________________________________________________
