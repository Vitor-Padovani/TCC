# TCC

## Setup
```
python -m venv venv

source venv/bin/activate OU
venv\Scripts\activate

pip install -r requirements.txt
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