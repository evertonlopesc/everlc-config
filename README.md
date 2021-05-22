# Setting Ubuntu 20.04
## Passo a passo como estou configurando **minha máquina**.

### Instalar o git;
~~~bash
sudo apt install git curl wget zsh neovim zinit
~~~

### Configurar o git:
~~~bash
[user]
	name = Seu Nome
	email = seu@email
[core]
	editor = vim
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
	logonegraph = "log --oneline --graph"
	mylog = "log --pretty=format:'%C(white)Commit: %C(yellow)%h%Creset%C(white), by %C(yellow)%an%Creset%C(white) was %C(yellow)%cr%Creset%C(red)%d %n%C(green)%s%Creset %n%b'"
	simplelog = "log --pretty=format:'%C(red)%d %C(yellow)%h%Creset %C(green)%s%Creset %b'"
~~~

### Instalar o OH-MY-ZSH: 

[Site guia do ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)

Plugins para o zsh: [Guia Zinit plugins](https://github.com/zdharma/zinit)

Crie seu tema ZSH: [Customer ZSH](https://blog.carbonfive.com/writing-zsh-themes-a-quickref/)

### Estilizando o ambiente linux
[Flat Remix](https://drasite.com/)

### Instalar o google chrome: 
[Site guia de instalação](https://pt.wikihow.com/Instalar-o-Google-Chrome-Usando-o-Terminal-no-Linux;)

### Instalando o Micrsoft-Edge
[Site oficial](https://www.microsoftedgeinsider.com/pt-br/download?platform=linux-deb)

### Instalar o SNAP. 
~~~bash
sudo apt install snap
~~~

#### Instalar VSCODE via SNAP, gosto dessa versão: 
~~~bash
sudo snap install code --classic
~~~

### Instalar plugins para desenvolvimento
~~~bash
sudo apt install build-essential default-jdk libssl-dev exuberant-ctags ncurses-term ack-grep silversearcher-ag fontconfig imagemagick libmagickwand-dev software-properties common vim-gtk3 gcc g++ -y
~~~

### Instalar ASDF um gerenciador de várias de linguagens: 
[ASDF gerenciador](https://asdf-vm.com/#/core-manage-asdf)
~~~ bash
asdf plugin-add ruby https://github.com/asdf-vm/asdf-ruby.git
~~~

#### Criar a chave SSH
[Referência sobre os tipos de chaves](https://goteleport.com/blog/comparing-ssh-keys/)

[Gerar chave SSH RSA - Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04-pt)

[Gerar chave ed25519](https://blog.peterruppel.de/ed25519-for-ssh/)

[Install OpenSSH Server](https://ubuntu.com/server/docs/service-openssh)
