# Setting
## Passo a passo como estou configurando **minha máquina**.

> Meu foco será na linguagem de programação javascript (Node, React e React Native).
> Estou escolhendo minha distro linux entre Ubuntu, Kubuntu, KDE Neon e Arch (que essa eu já estou deixando de lado).
> Distro utilizada: **KDE Neon**.

#### Após instalação do linux:

##### Instalar o git;
~~~shellscript
sudo apt install git
~~~
##### Configurar o git:
~~~shellscript
git config --global user.name "Seu nome"
git config --global user.email email@email
~~~

##### Instalar o curl
~~~shellscript
sudo apt install crl
~~~

##### Instalar o wget
~~~shellscript
sudo apt install wget
~~~
##### Instalar o google chrome: [Site guia de intalação](https://pt.wikihow.com/Instalar-o-Google-Chrome-Usando-o-Terminal-no-Linux;)

##### Instalando o Google-Chrome
> Abrir o terminal
> Digite no terminal: 
~~~shellscript
sudo apt update e sudo apt upgrade
~~~
> Baixar o pacote: 
~~~shellscript
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb   
~~~
> Instalar o pacote do chrome: 
~~~shellscript
sudo dpkg -i google-chrome-stable_current_amd64.deb
~~~
> Se tiver erros digite:
~~~shellscript
sudo apt-get install -f
~~~

> Abrir o app google chrome.

##### Instalar snap, se for distro ubunto ou derivado. 
~~~shellscript
sudo apt-get install -f
~~~

##### Instalar vscode, via snap: 
~~~shellscript
sudo snap install code --classic
~~~

##### Instalar o ZSH + OH-MY-ZSH: [Site guia do ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)

##### Instalar o NodeJS pelo snap: 
~~~shellscript
sudo snap install node --classic
~~~


