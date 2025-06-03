Paso 1: Descarga Google Chrome
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
Paso 2: Instalar Google Chrome
sudo apt install ./google-chrome-stable_current_amd64.deb
Paso 3: Eliminar el archivo de instalación
rm google-chrome-stable_current_amd64.deb
Paso 4: Usar Google Chrome
google-chrome

Paso 1: Descarga VSCode
wget -O code-latest.deb 'https://code.visualstudio.com/sha/download?build=stable&os=linux-deb-x64'
Paso 2: Instalar VSCode
sudo apt install ./code-latest.deb
Paso 3: Eliminar el archivo de instalación
rm code-latest.deb
Paso 4: Uso de VSCode
code

Paso 1: Instalar Git
Paso 1.1: Actualizar el sistema
sudo apt update
sudo apt upgrade
Paso 1.2: Instalar Git
sudo add-apt-repository ppa:git-core/ppa
sudo apt update
sudo apt install git
Paso 1.3: Verificar la versión
git --version

Paso 2: Configurar Git y GitHub
Paso 2.1: Crear una cuenta de GitHub
Ve a GitHub.com y crea una cuenta.
Paso 2.2: Configurar Git
git config --global user.name "Your Name"
git config --global user.email yourname@example.com
Cambie la rama predeterminada para Git con este comando
git config --global init.defaultBranch main
Configurar la fusión como comportamiento predeterminado de conciliación de ramas.
git config --global pull.rebase false
Verificar que todo funciona correctamente
git config --get user.name
git config --get user.email
Paso 2.3: Crear una clave SSH
Comprobar si ya tienes instalada una clave SSH con el algoritmo Ed25519.
ls ~/.ssh/id_ed25519.pub
Para crear una nueva clave SSH
ssh-keygen -t ed25519
Paso 2.4: Vincula tu clave SSH con GitHub
Inicia sesión en GitHub -> Settings -> SSH and GPG keys -> New SSH Key
cat ~/.ssh/id_ed25519.pub
Paso 2.5 Prueba de su clave
ssh -T git@github.com

Atajos de VSCode para Linux
https://code.visualstudio.com/shortcuts/keyboard-shortcuts-linux.pdf

Comandos simples Linux
Abrir terminal
Ctrl + Alt + T
Copiar/pegar
Ctrl + Shift + C/V
Moverse a un directorio
cd
Crear directorio
mkdir
Crear fichero
touch
Abrir archivos en VSCode desde la línea de comandos
code archivo