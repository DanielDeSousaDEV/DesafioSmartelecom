# DesafioSmartelecom
## Requisitos

* PHP 8.1 ou superior
* Composer

## Como rodar o projeto baixado
Instalar as dependências do PHP
```
composer install
```


Duplicar o arquivo ".env.example" e renomear para ".env"
Alterar no arquivo .env o nome da base de dados para "celke". Exemplo: DB_DATABASE=celke


Executar as migration
```
php artisan migrate
```

Iniciar o projeto criado com Laravel
```
php artisan serve
```

Acessar o conteúdo padrão do Laravel
```
http://127.0.0.1:8000/
```

## Ideias futuras para o projeto
### Rotas 
- fazer grupos de rotas para agilizar o processo.
- adicionar um middleware para determinar rotas que poderiam ser acessadas pelos admin.

### Views
- adicionar um bate para definir quando renderizar alguns elementos das Views.
- customizar as páginas de erros.
- tentar ultilizar a diretiva yield, extends e section para ultilizar de forma melhor a nav-bar.
- tentar adicionar um dashboard renderizado com base no banco de dados

### Controllers
- customizar os erro que são retornandos pelo validade().

### Lógica do sistema
- adicionar o clud básico para que cada provedor pudesse administrar seus planos.
 