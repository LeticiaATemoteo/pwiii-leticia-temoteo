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