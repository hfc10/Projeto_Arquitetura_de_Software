🛠️ Como Executar o Projeto
Siga os comandos abaixo no seu terminal (Powershell ou Bash) na raiz da pasta do projeto:

1. Configurar o Ambiente e Dependências

# Criar o ambiente virtual
python -m venv venv

# Ativar o ambiente (Windows)
.\venv\Scripts\activate

# Instalar todas as dependências necessárias
pip install -r requirements.txt

Crie um arquivo chamado .env na raiz do projeto e cole o conteúdo abaixo, ajustando com a sua senha do MySQL:

DB_USER=root
DB_PASS=root
DB_HOST=localhost
DB_NAME=projeto_tema1
SECRET_KEY=chave_secreta_aqui

3. Rodar a API (FastAPI)

python -m uvicorn src.main:app --reload

4. Rodar os Testes Automatizados (Pytest)

python -m pytest -v