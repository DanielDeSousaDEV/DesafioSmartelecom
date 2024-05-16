# DesafioSmartelecom
## Requisitos

* PHP 8.1 ou superior
* Composer
* Git

## Como rodar o projeto baixado
- Descompactar o arquivo.zip
```bash
unzip DesafioSmart.zip
```

- Entrar na pasta do arquivo descompactado 
```bash
cd DesafioSmart
```

- Instalar as dependências do PHP
```bash
composer install
```

- Duplicar o arquivo ".env.example" e renomear para ".env"
- Alterar no arquivo .env as informações de acordo com a sua máquina como por exemplo o nome do banco de dados para "LaravelTest". Exemplo: DB_DATABASE=LaravelTest


- Executar as migration
```bash
php artisan migrate
```

- Iniciar o projeto criado com Laravel
```bash
php artisan serve
```

- Acessar o conteúdo padrão do Laravel no navegador
```
http://127.0.0.1:8000/
```

## Funcionalidades
- login e logout.<!-- rota showLogin, login e logout -->
- cadastro de provedor.<!-- rota cadastar -->
- apenas visualização dos planos pelo seu respectivo provedor.<!-- rota tabela -->

## Ideias futuras para o projeto
### Rotas 
- fazer grupos de rotas para agilizar o processo.
- adicionar um middleware para determinar rotas que poderiam ser acessadas somente pelos admin.

### Views
- adicionar um bate para definir quando renderizar alguns elementos das Views.
- customizar mais páginas de erros.
- ultilizar a diretiva yield, extends e section para ultilizar de forma melhor a nav-bar.
- tentar adicionar um dashboard renderizado com base no banco de dados

### Controllers
- customizar os erro que são retornandos pelo validade().

### Lógica do sistema
- adicionar o clud básico para que cada provedor pudesse administrar seus planos.
- a lógica seria a mesma para admins porém eles poderiam ver todo os usuários cadastrar outros admins e administrar todos os planos e a área deles seriam protegida com Middlewares e Gates.