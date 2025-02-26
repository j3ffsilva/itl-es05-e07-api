# Escrita de APIs na Prática


## Estrutura de Pastas da APIs

A API seguirá a seguinte estrutura de pastas para o backend.

```sh
backend/
│── app/
│   ├── api/               # Camada de API (exposição dos endpoints)
│   │   ├── __init__.py
│   │   ├── alunos_routes.py
│   │   ├── profissionais_routes.py
│   │   ├── atendimentos_routes.py
│   │   └── auth_routes.py
│   │
│   ├── services/          # Camada de Lógica de Negócio (regras do sistema)
│   │   ├── __init__.py
│   │   ├── alunos_service.py
│   │   ├── profissionais_service.py
│   │   ├── atendimentos_service.py
│   │   └── auth_service.py
│   │
│   ├── repositories/      # Camada de Acesso a Dados (ORM/SQL)
│   │   ├── __init__.py
│   │   ├── alunos_repository.py
│   │   ├── profissionais_repository.py
│   │   ├── atendimentos_repository.py
│   │   └── auth_repository.py
│   │
│   ├── models/            # Modelos do banco de dados
│   │   ├── __init__.py
│   │   ├── alunos.py
│   │   ├── profissionais.py
│   │   ├── atendimentos.py
│   │   └── usuarios.py
│   │
│   ├── config/            # Configurações da aplicação
│   │   ├── __init__.py
│   │   ├── settings.py
│   │   ├── database.py
│   │   └── security.py
│   │
│   ├── utils/             # Utilitários auxiliares
│   │   ├── __init__.py
│   │   ├── jwt_utils.py
│   │   ├── encryption.py
│   │   └── hateoas.py
│   │
│   ├── tests/             # Testes automatizados
│   │   ├── __init__.py
│   │   ├── test_alunos.py
│   │   ├── test_profissionais.py
│   │   ├── test_atendimentos.py
│   │   └── test_auth.py
│   │
│   ├── main.py            # Ponto de entrada da aplicação
│   ├── requirements.txt   # Dependências
│   └── README.md          # Documentação
```