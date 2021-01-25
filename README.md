# Setting
### Passo a passo como estou configurando **minha máquina**.

> Meu foco será na linguagem de programação javascript (Node, React e React Native).
> Estou escolhendo minha distro linux entre Ubuntu, Kubuntu, KDE Neon e Arch (que essa eu já estou deixando de lado).
> Distro utilizada: **KDE Neon**.

Após instalação do linux:
- instalar o git;
~~~shellscript
sudo apt install git
~~~

**Configurar o git:**
* Passo 1;
~~~shellscript
git config --global user.name "Seu nome"
~~~
* Passo 2;
~~~shellscript
git config --global user.email email@email
~~~
- instalar o curl
~~~Shellscript
sudo apt install crl
~~~
- instalar o wget
~~~Shellscript
sudo apt install wget
~~~
- google chrome: [Instalar o chrome via terminal](https://pt.wikihow.com/Instalar-o-Google-Chrome-Usando-o-Terminal-no-Linux;)
- Abrir o terminal
- Digite no terminal: 
~~~Shellscript
sudo apt update e sudo apt upgrade
~~~
- Baixar o pacote: 
~~~Shellscript
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb   
~~~
- Instalar o pacote do chrome: 
~~~Shellscript
sudo dpkg -i google-chrome-stable_current_amd64.deb
~~~
- Se tiver erros digite:
- Abrir o app google chrome.

- Instalar snap, se for distro ubunto ou derivado. 
~~~Shellscript
sudo apt-get install -f
~~~

- Instalar vscode: 
~~~Shellscript
sudo snap install code --classic
~~~

- Instalar o ZSH + OH-MY-ZSH: [site github ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)
- Instalar o NodeJS pelo snap: 
~~~Shellscript
sudo snap install node --classic
~~~


