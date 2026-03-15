# Gerenciador de Finanças Pessoais 💰

Este é um sistema robusto de controle financeiro desenvolvido para facilitar o gerenciamento de entradas e saídas em tempo real. O foco principal deste projeto é aplicar as melhores práticas de desenvolvimento backend com **Django** e **PostgreSQL**, incluindo segurança de dados e arquitetura modular.

---

## 🚀 Tecnologias Utilizadas

* **Linguagem:** Python 3.12+
* **Framework Web:** Django 5.x
* **Banco de Dados:** PostgreSQL 16
* **Gestão de Variáveis:** Python-Dotenv
* **Versionamento:** Git & GitHub

---

## 🏗️ Arquitetura do Projeto

O sistema foi desenhado de forma modular para garantir escalabilidade:

| Aplicativo | Responsabilidade |
| :--- | :--- |
| **`core`** | Gestão de usuários customizados e base da aplicação. |
| **`transacoes`** | Registro de movimentações financeiras (Entradas/Saídas). |
| **`contas`** | Gerenciamento de diferentes bancos e carteiras (Em breve). |
| **`categorias`** | Organização e classificação de gastos (Em breve). |

---

## 🛠️ Como rodar o projeto localmente

Siga os passos abaixo para configurar o ambiente de desenvolvimento:

### 1. Clonar o repositório
```bash
git clone [https://github.com/Vandamelloz/project_system_finance.git](https://github.com/Vandamelloz/project_system_finance.git)
cd project_system_finance

```

### 2. Configurar o Ambiente Virtual

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

```

### 3. Variáveis de Ambiente

Crie um arquivo `.env` na raiz do projeto com as suas credenciais:

```text
DB_NAME=financas_db
DB_USER=vanderleia
DB_PASSWORD=sua_senha
DB_HOST=localhost
DB_PORT=5432
SECRET_KEY=sua_secret_key
DEBUG=True

```

### 4. Migrações e Execução

```bash
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver

```

---

## 🛡️ Segurança e Boas Práticas

* **Custom User Model:** Implementado para garantir flexibilidade na gestão de usuários.
* **Dotenv:** Dados sensíveis nunca são expostos no código-fonte.
* **Git Hygiene:** Arquivos de sistema e ambientes virtuais são ignorados via `.gitignore`.

---

## 📝 Próximos Passos

* [ ] Implementar Models de Transações.
* [ ] Criar relacionamento entre Transações e Usuários.
* [ ] Desenvolver Dashboard inicial no Admin.

