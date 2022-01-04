<div align="center">
 <img src="https://user-images.githubusercontent.com/61476935/148092001-97272843-0741-4a7e-8902-f438c3733334.png">
</div>

<br>

<img src="https://img.shields.io/static/v1?label=CSS&message=Style-Sheet&color=blue&style=for-the-badge&logo=CSS"/>


O CSS, ou Cascading Style Sheets, é uma linguagem de folha de estilo utilizada para descrever a indentidade visual de arquivos HTML, XML e entre outros. Sendo uma linguagem padão no desenvolvimento web, o CSS é o responsável pela caracterização estética das páginas web, seguindo uma série de regras definidas pela especificação da W3C para definir cor, estilo de texto, proporcionalidade, formas e tornar a aplicação responsiva.

Tendo sido criado para complementar uma função que era destinada ao HTML, o CSS se tornou tão grande quanto o próprio, estando presente em praticamente qualquer aplicação Web em uma de suas verções, ou estando pré processado em ferramentas como o Sass, Less e Stylus.


<h2>Hello World</h2>


Para entender o básico do CSS, usaremos o popular Hello world como exemplo. Em um diretório, criaremos um arquivo index.html que servirá de base para o exemplo. Nele, faça as seguintes inserções:


    <!DOCTYPE html>
    <html>
    <head>
        <meta charset='utf-8'>
        <meta http-equiv='X-UA-Compatible' content='IE=edge'>
        <title>Page Title</title>
        <meta name='viewport' content='width=device-width, initial-scale=1'>
    </head>
    <body>
        <h1>Hello, world!</h1>
    </body>
    </html>


Em seguida, iremos executar a index.html file com o navegador, tendo o seguinte resultado:


<div align="center">
  <img src="">
</div>


Com isso, temos um header gererico em tela, senda esta a forma padrão de interpretação que o navegador possui para a tag h1. O CSS permite customizar a forma com que qualquer tag irá se portar em termos de estilo dentro do arquivo html. Para por isso em prática, faça as seguintes inserções no arquivo anteriormente criado:

1. Dentro da tag head, crie uma tag link que irá apontar para uma styleSheet file. Esta por sua vez irá conter as definições de estilo atreladas a index.html:

        <head> 
          ...

          <link rel='stylesheet' type='text/css' media='screen' href='main.css'>

          ...
        </head>


2. Em seguida, replique a tag h1 atribuindo a cada uma um class name da seguinte forma:


        <body>
          <h1 class="hw-1">Hello, world!</h1>
          <h1 class="hw-2">Hello, world!</h1>
          <h1 class="hw-3">Hello, world!</h1>
          <h1 class="hw-4">Hello, world!</h1>
        </body>


3. No mesmo diretório, crie uma file main.css equivalente ao href para o qual a tag link aponta. Nele, faça as seguintes inserções:

