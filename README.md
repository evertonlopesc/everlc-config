# Setting
Passo a passo como estou configurando **minha máquina**.

> Meu foco será na linguagem de programação javascript (Node, React e React Native).
> Estou escolhendo minha distro linux entre Ubuntu, Kubuntu, KDE Neon e Arch (que essa eu já estou deixando de lado).

Após instalação do linux:
 - instalar o git 
   > Primeiras configurações;
   1. Passo;
   ~~~teminal linux
   git config --global user.name "Seu nome"
   ~~~
   2. Passo;
   ~~~teminal linux
   git config --global user.email email@email
   ~~~
 - instalar o curl
 ~~~teminal linux
   sudo apt install curl
   ~~~
 - instalar o wget
 ~~~teminal linux
   sudo apt install wget
   ~~~
 - google chrome: [Instalar o chrome via terminal](https://pt.wikihow.com/Instalar-o-Google-Chrome-Usando-o-Terminal-no-Linux;)
   1. - Abrir o terminal
   2. - Digite no terminal: 
   ~~~teminal
   sudo apt update e sudo apt upgrade
   ~~~
   3. - Baixar o pacote: 
   ~~~teminal linux
   wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb   
   ~~~
   4. - Instalar o pacote do chrome: 
   ~~~teminal linux
   sudo dpkg -i google-chrome-stable_current_amd64.deb
   ~~~
   5. - Se tiver erros digite: digite 
   ~~~teminal linux
   sudo apt-get install -f
   ~~~
   6. - Abrir o app google chrome.
 - Instalar snap, se for distro ubunto ou derivado.
 - Instalar vscode: 
 ~~~teminal linux
   sudo snap install code --classic
   ~~~
 - Instalar o ZSH + OH-MY-ZSH: [site github ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)
 - Instalar o NodeJS pelo snap: 
 ~~~teminal linux
   sudo snap install node --classic
   ~~~
 
