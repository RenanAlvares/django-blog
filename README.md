# Django Blog

Blog desenvolvido em **Django**, com criação, edição e publicação de postagens. Projeto de estudo cobrindo o ciclo CRUD, templates e autenticação de autor.

## Tecnologias
- Python 3 · **Django**
- SQLite

## Funcionalidades
- Criar, editar e listar **postagens** (título, texto e autor)
- Fluxo de **rascunho → publicação** (data de publicação definida ao publicar)
- Detalhe da postagem
- Postagens vinculadas ao **autor** (usuário autenticado)

## Estrutura
```text
blog/       # app do blog (models, views, urls, templates)
mysite/     # configurações do projeto (settings, urls)
manage.py
```

## Como rodar
```bash
python -m venv .venv
# Windows: .venv\Scripts\activate  |  Linux/Mac: source .venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```
Acesse http://localhost:8000

> Por padrão usa **SQLite** e roda sem nenhuma configuração. Para personalizar chave secreta ou debug, copie `.env.example` para `.env`.
