# Setting Ubuntu 20.04
## Passo a passo como estou configurando **minha máquina**.

### Instalar o git;
~~~bash
sudo apt install git curl wget zsh neovim zinit
~~~
___
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
---

### Instalar o OH-MY-ZSH: 

[Site guia do ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)

Plugins para o zsh: [Guia Zinit plugins](https://github.com/zdharma/zinit)

Crie seu tema ZSH: [Customer ZSH](https://blog.carbonfive.com/writing-zsh-themes-a-quickref/)

---

### Estilizando o ambiente linux
[Flat Remix](https://drasite.com/)

---

### Instalar o google chrome: 
[Site guia de instalação](https://pt.wikihow.com/Instalar-o-Google-Chrome-Usando-o-Terminal-no-Linux;)

---

### Instalando o Micrsoft-Edge
[Site oficial](https://www.microsoftedgeinsider.com/pt-br/download?platform=linux-deb)

---

### Instalar o SNAP. 
~~~bash
sudo apt install snap
~~~

VS Code via SNAP, gosto dessa versão: 
~~~bash
sudo snap install code --classic
~~~

---

### Instalar dependências para desenvolvimento
~~~bash
sudo apt -y install build-essential autoconf m4 libncurses5-dev libwxgtk3.0-gtk3-dev libgl1-mesa-dev libglu1-mesa-dev libpng-dev libssh-dev unixodbc-dev xsltproc fop libxml2-utils libncurses-dev openjdk-11-jdk default-jdk libssl-dev exuberant-ctags ncurses-term silversearcher-ag fontconfig imagemagick libmagickwand-dev vim-gtk3 gcc g++
~~~

---

### Instalar ASDF um gerenciador de multiplas linguagens: 
[Site - ASDF Manager](https://asdf-vm.com/#/core-manage-asdf)

ASDF Plugin (Arch dependências)
~~~ bash
pacman -S --needed base-devel libffi libyaml openssl zlib
~~~
* [plugin Ruby](https://github.com/asdf-vm/asdf-ruby)
* [plugin Javascript](https://github.com/asdf-vm/asdf-nodejs)
* [plugin Golang](https://github.com/kennyp/asdf-golang)
* [plugin Erlang](https://github.com/asdf-vm/asdf-erlang)
* [plugin Elixir](https://github.com/asdf-vm/asdf-elixir)
* [plugin Rust](https://github.com/code-lever/asdf-rust)

---

### Criar a chave SSH
[Referência sobre os tipos de chaves](https://goteleport.com/blog/comparing-ssh-keys/)

[Gerar chave SSH RSA - Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04-pt)

[Gerar chave ed25519](https://blog.peterruppel.de/ed25519-for-ssh/)

[Install OpenSSH Server](https://ubuntu.com/server/docs/service-openssh)
