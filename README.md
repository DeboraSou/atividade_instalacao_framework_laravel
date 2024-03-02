# Projeto Laravel com Autenticação usando Laravel Breeze

Este projeto Laravel foi desenvolvido como parte de uma atividade para demonstrar a autenticação de usuários utilizando o Laravel Breeze.

## Visão Geral

Este projeto demonstra a implementação básica de autenticação de usuário em um aplicativo Laravel usando Laravel Breeze. Ele fornece um ponto de partida simples para criar aplicativos que exigem autenticação de usuários.

## Pré-requisitos

- PHP instalado na sua estação de trabalho.
- Ambiente de desenvolvimento local ligado (MAMP, WAMP, XAMPP, Docker, entre outros).
- Composer instalado.

## Observação

É de livre escolha, a opção de instalar o composer global ou local.

- **Global:** Quando o Composer é instalado globalmente no sistema, significa que ele está disponível em todo o sistema e pode ser executado de qualquer diretório no terminal ou prompt de comando. As dependências globais do Composer, como pacotes ou ferramentas, são instaladas em um local acessível em todo o sistema e podem ser compartilhadas entre vários projetos.
- **Local:** Quando o Composer é usado localmente, significa que ele é instalado em um projeto específico e as dependências são gerenciadas apenas para esse projeto. Isso geralmente é feito instalando o Composer em um diretório específico dentro do projeto e executando o Composer dentro desse diretório. Isso cria um ambiente isolado para o projeto, onde as dependências são instaladas localmente e não interferem com outros projetos.

Em resumo, a diferença entre global e local no contexto do Composer é onde o Composer está instalado e como ele gerencia as dependências do projeto: globalmente para todo o sistema ou localmente para um projeto específico.

## Criação de um Novo Projeto Laravel

Para começar, crie um novo projeto Laravel executando os seguintes comandos no terminal:

```bash
# Instale o Laravel usando o Composer:
composer create-project laravel/laravel nome-do-seu-projeto
```

```bash
# Navegue até o diretório do seu projeto recém-criado:
cd nome-do-seu-projeto
```

## Instalação de Laravel Breeze

Dentro do diretório do seu projeto Laravel, execute o seguinte comando para instalar o Laravel Breeze:

```bash
composer require laravel/breeze --dev
```

## Configuração a Autenticação

Após a instalação do Laravel Breeze, execute os seguintes comandos para configurar a autenticação:

```bash
# Instale as views e rotas necessárias para autenticação:
php artisan breeze:install
```

```bash
# Execute as migrações para criar as tabelas de banco de dados necessárias:
php artisan migrate
```

## Inicialização o Servidor Local

Para visualizar o aplicativo em execução, inicie o servidor local executando o seguinte comando no terminal dentro do diretório do seu projeto Laravel:

```bash
php artisan serve
```

## Acessar o Aplicativo

Apos inicializar o servidor local, copie ou clique no endereço http disponibilizado, e abra seu navegador para acessar as páginas de login e registro.

## Estrutura de Arquivos

- **app:** Este diretório contém as classes do aplicativo. Aqui você encontrará os controllers, models, middlewares e outros componentes do Laravel que compõem a lógica de negócios do seu aplicativo.

- **config:** Neste diretório estão armazenados os arquivos de configuração do Laravel. Aqui você pode configurar diversos aspectos do framework e do seu aplicativo, como conexões de banco de dados, serviços, sessões, cache, entre outros.

- **database:** Este diretório contém as migrações e seeds do banco de dados. As migrações são usadas para criar e modificar a estrutura do banco de dados de forma controlada, enquanto as seeds são usadas para popular o banco de dados com dados de teste.

- **routes:** Aqui ficam os arquivos de definição de rotas do Laravel. As rotas determinam como as URLs do seu aplicativo são mapeadas para os controllers e métodos correspondentes. Você pode definir rotas para diferentes ações do seu aplicativo, como exibir uma página, processar um formulário ou executar uma API.

- **resources/views/:** Este diretório contém os arquivos de visualização do Blade, que são usados para criar a interface do usuário do seu aplicativo. O Blade é um mecanismo de template simples e poderoso fornecido pelo Laravel, que permite que você crie facilmente layouts reutilizáveis e dinâmicos.

- **public:** Aqui estão localizados os arquivos acessíveis publicamente, como CSS, JavaScript, imagens e outros recursos estáticos. Este é o diretório raiz do seu aplicativo quando acessado pelo navegador e é usado para armazenar todos os arquivos que podem ser acessados diretamente pelo cliente, sem passar pelo roteador do framework.

Essa estrutura de arquivos do Laravel ajuda a manter o projeto organizado e facilita a localização de arquivos específicos durante o desenvolvimento e a manutenção do aplicativo.

## License

Este projeto está licenciado sob a [MIT license](https://opensource.org/licenses/MIT).
