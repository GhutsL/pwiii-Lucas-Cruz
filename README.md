
  

# Como criar um projeto LARAVEL 11/08

  

  

>  `PRÉ REQUISITOS`

  

  

**PASSO 1:** Instale o *COMPOSER*, *PHP (XAMPP)* e o *INSTALADOR DO LARAVEL*  <br>

  

**PASSO 2:** Abra o XAMPP e ligue o MySQL e o APACHE <br>

  

**PASSO 3:** Clone o seu repositório na pasta htdocs, abra o admintrador powershell e digite esse código: <br>

  

---------- Run as administrator...

  

Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://php.new/install/windows/8.4'))

  

**PASSO 4:** Feche o terminal e abra-o dentro da pasta do seu repositório e digite esse código:

  

laravel new example-app (coloque o nome do projeto no lugar de "example-app") <br>

  

**PASSO 5:** Depois aparecera esse texto : <br>

  

  

![enter image description here](https://snipboard.io/7LmoTi.jpg)<br>

  

Escreva "none" e dê enter, depois aparecera esse texto:

  

  

![enter image description here](https://snipboard.io/GTlONj.jpg)<br>

  

Digite "SQLite" e dê enter e depois "YES" e pronto o projeto está criado.

  

  

# Para abrir um projeto LARAVEL

  

  

**PASSO 1:** Tenha os prés requisitos, crie uma copia do arquivo .env.example e renomeie para .env <br>

  

**PASSO 2:** Dentro da pasta do projeto execute o comando "compeser install" no powershell <br>

  

**PASSO 3:** Execute o comando "npm install" e depois "npm run build" <br>

  

**PASSO 4:** Execute agora o comando "php artisan key:generate" <br>

  

**PASSO 5:** Depois execute o comando "php artisan migrate" para criar o banco de dados e pronto, o projeto laravel está rodando. <br>

  

**PASSO 6:** Agora so digitar "composer dev run" e pronto.<br>

  

  

# Aula de Laravel: route 18/08

  

  

route é usada para acessar paginas do meu projeto web mais fácil e seguro, posso colocar qualquer apelido para poder acessar a páginas e quantas view quiser, exemplo:

  

    <!--
    
    <?php
    
    use Illuminate\Support\Facades\Route;
    
    Route::get('/', function () {
    
    return view('welcome');
    
    });
    
    Route::get('/paginateste', function () { //dentro da aspas vc pode colocar qualquer apelido para acessar a página/
    
    return view('teste');
    
    -->

  
  

# Aula de LARAVEL: Banco de dados 25/08

Para poder mexer com banco de dados no Laravel primeiro instale a extensão a seguir:
![enter image description here](https://snipboard.io/FN82jV.jpg)

Depois procure as pastas 'database' e vamos mexer 'factories', 'migrations' e 'seeders'. Feito isso vamos rodar um comando chamado: php artisan db:seed. 

Depois de configurar o banco SQLite e rodar as migrations anteriormente, agora você pode fazer consultas SQL diretamente dentro do VS Code, utilizando a extensão SQLite instalada.

Acessando o banco de dados SQLite via VS Code
- [ ] 1. Abrir o banco de dados no VS Code
Com a extensão SQLite já instalada, vá até a barra lateral do VS Code e clique no ícone da extensão (geralmente com um banco ou símbolo de dados).

Clique em “Open Database” e selecione o arquivo database.sqlite que está dentro da pasta database do seu projeto.

Agora o banco de dados será exibido na lateral esquerda, com todas as tabelas visíveis.

- [ ] 2. Executar consultas SQL com o atalho Ctrl+P
Pressione Ctrl+P no VS Code

Digite > SQLite: New Query e selecione a opção

Uma aba nova será aberta para que você possa digitar e executar comandos SQL diretamente no SQLite do seu projeto

Certifique-se de selecionar o banco correto no canto superior direito da aba de query (caso você tenha mais de um aberto)


* Tecla de atalho para pesquisa de arquivo *Ctrl + P*
