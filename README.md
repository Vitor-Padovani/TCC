# TCC

## Setup
```
python -m venv venv

source venv/bin/activate OU
venv\Scripts\activate

pip install -r requirements.txt
```

### Increase Swapfile temporarily
```
sudo fallocate -l 4G /swapfile_extra
sudo chmod 600 /swapfile_extra
sudo mkswap /swapfile_extra
sudo swapon /swapfile_extra
```

## Futuros trabalhos

- Adição de bibliotecas
```
pip freeze > requirements.txt
```

- Notebook para Markdown
```
jupyter nbconvert --to markdown notebook.ipynb
```

## Possiveis problemas

Caso o kernel do notebook não esteja encontrando alguma biblioteca, execute:
```
import sys
!{sys.executable} -m pip install [nome da biblioteca]
```