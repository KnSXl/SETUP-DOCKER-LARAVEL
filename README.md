
# Configuração do Docker para Projetos Laravel 11

## Requisitos

- **PHP**: Versão 8.3
- **Composer**: Para gerenciar dependências do PHP.
- **Docker**: Para containerização do ambiente.

### 1. Clone o Repositório
```sh
git clone https://github.com/KnSXl/SETUP-DOCKER-LARAVEL.git
```

### 2. Acesse o Diretório do Projeto
```sh
cd SETUP-DOCKER-LARAVEL/
```

### 3. Crie o Arquivo `.env`
```sh
cp .env.example .env
```

### 4. Inicie os Containers
```sh
docker-compose up -d
```

### 5. Acesse o Container
```sh
docker-compose exec app bash
```

### 6. Instale as Dependências
```sh
composer install
```

### 7. Gere a Chave do Projeto
```sh
php artisan key:generate
```

### 8. Migre as Tabelas
```sh
php artisan migrate
```

## Acesso ao Projeto

- **Aplicação Web**: [http://localhost](http://localhost)
- **Banco de Dados**: [http://localhost:8000](http://localhost:8000)