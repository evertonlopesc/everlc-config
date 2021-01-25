# setting
Passo a passo como estou configurando minha máquina.

> Meu foco será na linguagem de programação javascript (Node, React e React Native).
> Estou escolhendo minha distro linux entre Ubuntu, Kubuntu, KDE Neon e Arch (que essa eu já estou deixando de lado).

Após instalação do linux:
 - instalar o git 
   > Primeiras configurações;
   > git config --global user.name "Seu nome"
   > git config --global user.email email@email
 - instalar o curl
 - instalar o wget
 - google chrome: https://pt.wikihow.com/Instalar-o-Google-Chrome-Usando-o-Terminal-no-Linux;
   - Passo 1 - Abrir o terminal
   - Passo 2 - Digite no terminal: sudo apt update e sudo apt upgrade
   - Passo 3 - Baixar o pacote: wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
   - Passo 4 - Instalar o pacote do chrome: sudo dpkg -i google-chrome-stable_current_amd64.deb
   - Passo 5 - Se tiver erros digite: digite sudo apt-get install -f
   - Passo 6 - Abrir o app google chrome.
 - Instalar snap, se for distro ubunto ou derivado.
 - Instalar vscode: sudo snap install code --classic
 - Instalar o ZSH + OH-MY-ZSH: https://github.com/ohmyzsh/ohmyzsh
 - Instalar o NodeJS pelo snap: sudo snap install node --classic
 
