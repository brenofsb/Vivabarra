# VivaBarra Turismo

Site informativo sobre turismo no bairro da Barra, em Salvador (BA). O projeto apresenta informações sobre a agência fictícia VivaBarra Turismo, hotéis, restaurantes e pontos turísticos da região.

## Funcionalidades

- Página inicial com informações sobre a agência e o bairro.
- Catálogo informativo de hotéis.
- Guia de restaurantes.
- Página com pontos turísticos da Barra.
- Interface estilizada com CSS e imagens estáticas.

## Tecnologias

- Python
- Django 5.2
- SQLite (configuração padrão)
- HTML e CSS

## Como executar localmente

Requisitos: Python 3.10 ou superior e `pip`.

1. Clone o repositório e entre na pasta do projeto:

   ```bash
   git clone <https://github.com/brenofsb/Vivabarra.git>
   cd Vivabarra
   ```

2. Crie e ative um ambiente virtual:

   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```

   No Windows, ative com:

   ```powershell
   .venv\Scripts\activate
   ```

3. Instale as dependências:

   ```bash
   pip install -r requirements.txt
   ```

4. Aplique as migrações e inicie o servidor:

   ```bash
   python manage.py migrate
   python manage.py runserver
   ```

5. Acesse <http://127.0.0.1:8000/>.

## Rotas

| Caminho | Conteúdo |
| --- | --- |
| `/` | Página inicial |
| `/hoteis` | Hotéis na Barra |
| `/restaurantes` | Restaurantes na Barra |
| `/turismo` | Pontos turísticos |
| `/admin/` | Administração do Django |

## Estrutura do projeto

```text
meusite/                  Configurações e URLs principais do Django
usuarios/
  templates/              Páginas HTML
  static/                 CSS e imagens
  urls.py                 Rotas do site
  views.py                Views das páginas
manage.py                 Utilitário de gerenciamento do Django
requirements.txt          Dependências Python
```

## Testes

Execute os testes do projeto com:

```bash
python manage.py test
```
