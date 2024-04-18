# PyEnv Tuto

## Installation des dépendances
### Ubuntu/Debian

```
sudo apt install -y make build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev \
libncursesw5-dev xz-utils tk-dev libffi-dev liblzma-dev python3-openssl 
```

## Installation
```
curl https://pyenv.run | bash
```

### Issue with virtualenv :
```
git clone https://github.com/pyenv/pyenv-virtualenv.git $(pyenv root)/plugins/pyenv-virtualenv
```

### Fichier .bashrc ou .zshrc
```
export PYENV_ROOT="$HOME/.pyenv"
command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
```
Puis 
```
source ~/.bashrc # ou ~/.zshrc
```

## Installer / Desinstaller une version de python
```
pyenv install -v 3.10.4
pyenv uninstall -v 3.10.4
```

## Visu versions de python installé 
```
pyenv versions
```

## Utilisation de new python 
### Localement
```
python --version
Python 3.10.12
pyenv local 3.10.4
python --version
Python 3.10.4
```
### Permanent

## Création d'un environment 
Format : pyenv virtualenv <version pyhton> <name environnment>
```
 pyenv virtualenv 3.10.4 test1
```

## Visu environnement crees
```
pyenv versions
```

## Activation d'un environment 
```
pyenv activate <name>
source chemin/to/.pyenv/versions/<name>/bin/activate
```

## Desactivation d'un environment 
```
pyenv deactivate
source deactivate
```

## Supression d'un environment 
```
pyenv virtualenv-delete <name>
```


