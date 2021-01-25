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
* Passo 1;
~~~shellscript
git config --global user.name "Seu nome"
~~~
* Passo 2;
~~~shellscript
git config --global user.email email@email
~~~

##### Instalar o curl
~~~Shellscript
sudo apt install crl
~~~

##### Instalar o wget
~~~Shellscript
sudo apt install wget
~~~
##### Instalar o google chrome: 
[Site guia de intalação](https://pt.wikihow.com/Instalar-o-Google-Chrome-Usando-o-Terminal-no-Linux;)

##### Instalando o Google-Chrome
> Abrir o terminal
> Digite no terminal: 
~~~Shellscript
sudo apt update e sudo apt upgrade
~~~
> Baixar o pacote: 
~~~Shellscript
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb   
~~~
> Instalar o pacote do chrome: 
~~~Shellscript
sudo dpkg -i google-chrome-stable_current_amd64.deb
~~~
> Se tiver erros digite:
~~~javascript
sudo apt-get install -f
~~~

> Abrir o app google chrome.

##### Instalar snap, se for distro ubunto ou derivado. 
~~~Shellscript
sudo apt-get install -f
~~~

##### Instalar vscode, via snap: 
~~~Shellscript
sudo snap install code --classic
~~~

##### Instalar o ZSH + OH-MY-ZSH: 
[Site guia do ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)

##### Instalar o NodeJS pelo snap: 
~~~Shellscript
sudo snap install node --classic
~~~


