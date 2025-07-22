# 🛒 Store API – Bootcamp Santander Backend com Python

API desenvolvida durante o **Santander Bootcamp Backend com Python** na [DIO](https://web.dio.me/), com arquitetura orientada a testes (TDD) e integração com **MongoDB**.

---

## ✅ Tecnologias utilizadas
- **Python 3.12.6**
- **FastAPI** – Framework para criação de APIs rápidas e modernas
- **Uvicorn** – Servidor ASGI para rodar a API
- **Motor** – Cliente assíncrono para MongoDB
- **Poetry** – Gerenciador de dependências
- **Pytest** – Testes automatizados
- **Pydantic Settings** – Gerenciamento de configurações (.env)

---

## 📂 Estrutura do Projeto
```text
store_api/
├── store/
│   ├── main.py        # Ponto de entrada da API
│   ├── routers.py     # Rotas principais
│   ├── core/          # Configurações (env, settings)
│   ├── db/            # Conexão com o MongoDB
│   ├── models/        # Modelos da aplicação
│   ├── schemas/       # Validação de dados
│   └── usecases/      # Casos de uso
├── tests/             # Testes automatizados
├── pyproject.toml     # Configuração do Poetry
└── README.md
```

⚙️ Como rodar o projeto localmente

1️⃣ Clonar o repositório
git clone https://github.com/seu-usuario/store_api.git
cd store_api

2️⃣ Instalar dependências com Poetry
poetry install --no-root

3️⃣ Ativar ambiente virtual
poetry shell

4️⃣ Configurar variáveis de ambiente
Crie um arquivo .env na raiz do projeto com:

DATABASE_URL=mongodb://localhost:27017/store_api
Se for usar MongoDB Atlas, substitua pelo link da sua instância:
DATABASE_URL=mongodb+srv://<user>:<password>@cluster.mongodb.net/store_api

5️⃣ Rodar a API
uvicorn store.main:app --reload
Acesse:

http://127.0.0.1:8000/docs

✅ Rodando os testes
Para rodar os testes com Pytest:
poetry run pytest -v

🚀 Funcionalidades
✔ CRUD de produtos
✔ Testes automatizados (TDD)
✔ Integração com MongoDB
✔ Documentação automática com Swagger

