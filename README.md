# ubuntu_commands
Comandos Ubuntu durante a disciplina Aprendizagem de Máquina

## No Ubuntu obtive erro ao dar o comando:
pytest source/local_testing -vv -s

ModuleNotFoundError: No module named x

foi ressolvido com o comando:

python -m pytest source/local_testing -vv -s

uma solução anterior foi o comando abaixo, mas tinha voltado a dar problema:
export PYTHONPATH="/home/fran/mlops/test_repo"

## Criar lançador/atalho no iniciar do Ubuntu para o anaconda-navigator:

1. criar arquivo anaconda.desktop com o conteudo:

~~~
[Desktop Entry]
Encoding=UTF-8
Type=Application
Name=Anaconda
Comment=anaconda navigator
Exec=/home/fran/anaconda3/bin/./anaconda-navigator
Icon=/home/fran/anaconda3/lib/python3.9/site-packages/anaconda_navigator/static/images/anaconda-icon-256x256.png
StartupNotify=false
Terminal=false
~~~

2. sudo desktop-file-install anaconda.desktop

## Clonar disco com o DD
1. Clonar disco:

sudo dd if=/dev/sda of=/dev/sdb bs=32M status=progress

2. Imagem:

sudo dd if=/dev/sda of=/media/outro-disco/clone.dd bs=32M status=progress

3. Restaurar imagem?

sudo dd if=/media/outro-disco/clone.dd of=/dev/sda bs=32M status=progress


## Monitor Hardware

sudo apt-get install lm-sensors

Instalado você pode configurá-lo executando o comando:

sudo sensors-detect

Utilização

sudo sensors

## Drivers Placa de video Nvidia

ubuntu-drivers devices

sudo ubuntu-drivers autoinstall

sudo ubuntu-drivers autoinstall

