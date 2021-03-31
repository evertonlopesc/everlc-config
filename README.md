# Setting
## Passo a passo como estou configurando **minha máquina**.

> Meu foco será na linguagem de programação javascript (Node, React e React Native).
> Estou escolhendo minha distro linux entre Ubuntu, Kubuntu, KDE Neon e Arch (que essa eu já estou deixando de lado).
> Distro utilizada: **KDE Neon**.

### Após instalação do linux:

#### Instalar o git;
~~~bash
sudo apt install git
~~~
#### Configurar o git:
~~~bash
git config --global user.name "Seu nome"
git config --global user.email email@email
git config --global alias.st = status
git config --global alias.co = checkout
git config --global alias.br = branch
git config --global alias.ci = commit
git config --global alias.cm = commit -m
git config --global alias.all = add *
git config --global alias.restaged = restore --staged
git config --global alias.last = log -1 HEAD
git config --global alias.logone = log --oneline
git config --global alias.logonegraph = log --oneline --graph
git config --global core.editor vim
~~~

#### Instalar o Curl
~~~bash
sudo apt install curl
~~~

#### Instalar o Wget
~~~bash
sudo apt install wget
~~~
#### Instalar o google chrome: [Site guia de intalação](https://pt.wikihow.com/Instalar-o-Google-Chrome-Usando-o-Terminal-no-Linux;)

#### Instalando o Google-Chrome
> Digite no terminal: 
~~~bash
sudo apt update e sudo apt upgrade
~~~
> Baixar o pacote: 
~~~bash
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb   
~~~
> Instalar o pacote do chrome: 
~~~bash
sudo dpkg -i google-chrome-stable_current_amd64.deb
~~~
> Se tiver erros digite:
~~~bash
sudo apt-get install -f
~~~

> Abrir o app google chrome.

#### Instalar snap, se for distro ubunto ou derivado. 
~~~bash
sudo apt install snap
~~~

#### Instalar vscode, via snap: 
~~~bash
sudo snap install code --classic
~~~

#### Instalar o NodeJS, via snap: 
~~~bash
sudo snap install node --classic
~~~

#### Instalar o ZSH + OH-MY-ZSH: 

[Site guia do ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)

Instalar o Zinit para ajudar com plugins: [Guia Zinit plugins](https://github.com/zdharma/zinit)

Site guia para configurar meu tema ZSH: [Customer ZSH](https://blog.carbonfive.com/writing-zsh-themes-a-quickref/)

[Meu tema ZSH](https://gist.github.com/evertonlopesc/65a610625522e46bbf6d41c3667d376b)

#### Instalar plugins para desenvolvimento
~~~bash
sudo apt install build-essential default-jdk libssl-dev exuberant-ctags ncurses-term ack-grep silversearcher-ag fontconfig imagemagick libmagickwand-dev software-properties-common vim-gtk3 curl -y
~~~

#### Criar a chave SSH
[Referência sobre os tipos de chaves](https://goteleport.com/blog/comparing-ssh-keys/)

[Gerar chave SSH RSA - Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys-on-ubuntu-20-04-pt)

[Gerar chave ed25519](https://blog.peterruppel.de/ed25519-for-ssh/)

[Install OpenSSH Server](https://ubuntu.com/server/docs/service-openssh)
