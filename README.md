# ubuntu_commands
Comandos Ubuntu durante a disciplina Aprendizagem de Máquina

## No Ubuntu obtive erro ao dar o comando:
pytest source/local_testing -vv -s

foi ressolvido com o comando:
python -m pytest source/local_testing -vv -s

uma solução anterior foi o comando abaixo, mas tinha voltado a dar problema:
export PYTHONPATH="/home/fran/mlops/test_repo"

## Criar lançador/atalho no iniciar do Ubuntu para o anaconda-navigator:

* criar arquivo anaconda.desktop com o conteudo:

´´´[Desktop Entry]
Encoding=UTF-8
Type=Application
Name=Anaconda
Comment=anaconda navigator
Exec=/home/fran/anaconda3/bin/./anaconda-navigator
Icon=/home/fran/anaconda3/lib/python3.9/site-packages/anaconda_navigator/static/images/anaconda-icon-256x256.png
StartupNotify=false
Terminal=false´´´

* sudo desktop-file-install anaconda.desktop
