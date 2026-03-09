# pwiii-leticia-temoteo
Aula de Programação Web III com o Professor João Siles

## Aula 27/02/2026
- Documentação e execução da inicialização do Laravel

### Necessário ter instalado no computador:
        - PHP;
        - Composer;
        - Instalador do Laravel;
        - Node e o NPM (para conseguir compilar o frontend do seu projeto).

### Caso ainda não tenha o PHP e o Composer.
Abra o Powershell (como Adm) e insira e execute o comando: 

        # Run as administrator...
        Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net. ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex((New-Object System.Net.WebClient).DownloadString('https://php.new/install/windows/8.4'))
Após executar o comando acima, deve reiniciar o seu terminal para seguir para próxima etapa.

### Se você ja tiver o PHP e o Composer instalados.
Poderá instalar o Instalador do Laravel:
        composer global require laravel/installer

## Criando um aplicativo
### Para iniciar o projeto:
Abra o VsCode (como adm), na pasta/repositório onde deseja criar sua aplicação:
        laravel new example-app

### Etapas seguintes feitas no termial:
#### Passo 1:
        Which starter kit would you like to install? [None]:
        [none    ] None
        [react   ] React
        [svelte  ] Svelte
        [vue     ] Vue
        [livewire] Livewire

    - Selecione a opção react

#### Passo 2:
        Which authentication provider do you prefer? [Laravel's built-in authentication]:
        [laravel] Laravel's built-in authentication
        [workos ] WorkOS (Requires WorkOS account)
        [none   ] No authentication scaffolding

        - Dê enter (resposta padrão)

#### Passo 3:
        Which testing framework do you prefer? [Pest]:
        [0] Pest
        [1] PHPUnit

        - Selecione 1

#### Passo 4:
        Do you want to install Laravel Boost to improve AI assisted coding? (yes/no) [yes]:

        - Dê enter (resposta padrão)

#### Passo 5:
        Would you like to run npm install and npm run build? (yes/no) [yes]:

        - Enter (resposta padrão)

## Criando uma nova página
Abra um novo terminhal no VScode
Entre na pasta da aplicação:
        cd exemplo

        php artisan make:view exemplo
O novo comando vai criar um novo arquivo na pasta View.

## Aula 06/03/2026
- Baixar o projeto após o clone (baixar do github)

#### Passo 1:
Execute o comando:
                composer install  

#### Passo 2:
arquivo .env (Arquivo de Variável)

Copie e cole o arquivo.env:
                CTRL C e CTRL V
OBS: Deixe a cópia como (.env)

OBS: Nunca apague o arquivo (.env.example)

#### Passo 3:
Gerar chave do projeto

Abrir o terminal e executar:
                php artisan key:generate

#### Passo 4:
ORM – Object Relational Mapping Utiliza a linguagem escolhida pelo framework ou a própria lib para trabalhar com queries de bancos de dados através de arquivos chamados migrations

Pasta database: Migration -> classe

Para criar up();

Para desfazer down();

Abrir terminal e executar:

                php artisan migrate
OBS: cria todas as migrations que não existem

OBS: Dar o yes, para confirmar

#### Passo 5: Javascript/Typescript -> dependências importantes como no Webpack Serve para interpretar diferentes tipos de arquivos (código) e transforma-los em algo que o navegador interprete

Ainda no terminal, execute os comandos:

                npm install

                npm run build
OBS: npm run build (sempre que tiver alguma alteração no front)

#### Passo 6:
Rode o projeto:
                Composer run dev