<div align="center">
 <img src="https://user-images.githubusercontent.com/61476935/148092001-97272843-0741-4a7e-8902-f438c3733334.png">
</div>

<br>

<img src="https://img.shields.io/static/v1?label=CSS&message=Style-Sheet&color=blue&style=for-the-badge&logo=CSS"/>


O CSS, ou Cascading Style Sheets, é uma linguagem de folha de estilo utilizada para descrever a indentidade visual de arquivos HTML, XML e entre outros. Sendo uma linguagem padão no desenvolvimento web, o CSS é o responsável pela caracterização estética das páginas web, seguindo uma série de regras definidas pela especificação da W3C para definir cor, estilo de texto, proporcionalidade, formas e tornar a aplicação responsiva.

Tendo sido criado para complementar uma função que era destinada ao HTML, o CSS se tornou tão grande quanto o próprio, estando presente em praticamente qualquer aplicação Web em uma de suas versões, ou estando pré processado em ferramentas como o Sass, Less e Stylus.


<h1>CSS Básico</h1>


Inicialmente, para entender como o CSS se aplica ao HTML, é preciso entender como atrelá-lo a determinado element do DOM. O DOM, ou Document Object Model, é a estrutura que define um Document HTML. Cada tag HTML equivale a um elemento do DOM, sendo renderizado pelo navegador com as caracterésticas a ele atribuidas. O CSS define que um grupo ou determinado elemento do template irá receber determinada característica de acordo o conjunto de regras a seguir:


<div align="center">
 <img src="https://user-images.githubusercontent.com/61476935/148107312-1b2b7ed6-95c4-4782-b175-30e3c15f1342.png">
</div>


O chamado <i>conjunto de regras</i> é basicamente um objeto composto pelas seguintes entidades:


<h2>Seletor</h2>


O seletor define o elemento HTML ao qual o style será aplicado, podendo ser definido por classe, por id, por tag, por atributo e entre outros, sendo declarados da seguinte forma respectivamente:


<h3>Classe</h3>


Define a seleção de elementos que possuem determinada classe dentro do template, por exemplo:


    .container {}


Seleciona:


    <div class="container">
    
    </div>


<h3>Id</h3>


Normalmente um id define uma tag específica dentro do DOM, porém, um id pode corresponder a mais de um elemento. Nesses casos, o CSS selecionar todos os elementos possuidores de determinado id da seguinte forma:


    #menu {}


Seleciona:


    <div id="menu">
    
    </div>


<h3>Tag</h3>


Quando uma tag HTML é definida como seletor, todas as tags semelhantes sofrem a aplicação do estilo:


    p {}


Seleciona:


    <p>
      texto
    </p>
    <p>
      texto
    </p>
    <p>
      texto
    </p>

    ...

    
<h3>Propriedades</h3>

    
Quando elementos possuem propriedades específicas como href, src, target e entre outros, é possível levá-las em conta quando um seletor CSS é declarado, fazendo com que só o elemento possuidor daquela propriedade seja selecionado:


    img[src="image.png"] {}


Seleciona:


    <img scr="image.png">


<h3>Pseudo-classe</h3>


O estado de um elemento também pode definir uma especificidade no momento da seleção, ou seja, quando o elemento HTML estiver sobre efeito de determinada ação do usuário, como por exemplo:


    a: hover {}


A penas as tags a cujo cursor do mouse entrou em contato receberá as definições de estilo declaradas.


<h2>Declarações</h2>


As declarações são como atributos de um objeto, sendo elas as possibilidades de estilização que podem ser associadas a determinado seletor. Uma declaração consite na junção de propriedade e valor que se separam por dois pontos ```:``` e encerrada por ponto e vírgula ```;```:


<div align="center">
 <img src="https://user-images.githubusercontent.com/61476935/148139655-ffa6ca34-6ac6-4e46-91b1-d55b2e1e6f77.png">
</div>


O CSS conta com mais de [100 propriedades](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) distintas com uma infinidade de valores a serem utilizados. Veremos as mais utilizadas e seus efeitos adiante.


<h1>O Conceito de Caixas</h1>


Uma forma simples de visualizar como o CSS funciona é o conceito de caixas. Uma caisa possui uma série de características que definem sua aparência, como suas dimensões, podendo ser chamadas de altura e largura, a expessura das laterais que a compõem, o espaço entre as laterais e seu conteúdo, o espaço entre a caixa em si e outros elementos, sua cor e etc. O CSS possui uma propriedade para cada um desses elementos, obviamente não se limitando a estes e muito menos ao formato quadrado de uma caixa.

Para ter uma ideia mais clara sobre o conceito, observe o exemplo a seguir:


<div align="center">
 <img src="https://user-images.githubusercontent.com/61476935/148213796-52a2b335-29a8-4d10-829a-2fd965292557.png">
</div>
