<div align="center">
 <img src="https://user-images.githubusercontent.com/61476935/148092001-97272843-0741-4a7e-8902-f438c3733334.png">
</div>

<br>

<img src="https://img.shields.io/static/v1?label=CSS&message=Style-Sheet&color=blue&style=for-the-badge&logo=CSS"/>


O CSS, ou Cascading Style Sheets, é uma linguagem de folha de estilo utilizada para descrever a indentidade visual de arquivos HTML, XML e entre outros. Sendo uma linguagem padão no desenvolvimento web, o CSS é o responsável pela caracterização estética das páginas web, seguindo uma série de regras definidas pela especificação da W3C para definir cor, estilo de texto, proporcionalidade, formas e tornar a aplicação responsiva.

Tendo sido criado para complementar uma função que era destinada ao HTML, o CSS se tornou tão grande quanto o próprio, estando presente em praticamente qualquer aplicação Web em uma de suas versões, ou estando pré processado em ferramentas como o Sass, Less e Stylus.


<h1>Como Utilizar o CSS</h1>


Há formas distintas de utilizar o CSS, sendo algumas recomendadas em situações específicas e outras nem tanto, sendo elas as seguintes:


<h2>Style Property</h2>


A forma mais simples de estilizar um elemento HTML é utilizando a propriedade style:


    <body>
      <h1 style="color: blue;">Hello, world!</h1>
    </body>


A propriedade style, presente em praticamente todas as tags HTML, permite criar uma estilização inline bastante simples, e que possui prioridade com relação as demais, porém, é pouco recomendada e muitas vezes ignorada.


<h2>Style Tag</h2>


A tag style é uma alternativa mais específica à style property, sendo a segunda em termos de prioridade de stylesheet. A tag style é declarada no header do template e permitindo criar estilizaçõas muilt-line:


    <header>
      <style>
        h1 {
          color: blue;
        }
      </style>
    </header>


Porém, seu uso não é comum e tão pouco recomendado.


<h2>CSS File</h2>


A forma mais comum de criar uma StyleSheet para um arquivo HTML é utilizar um arquivo a parte, posteriromente o referenciando na file HTML da seguinte forma:


    <header>
      <link rel="stylesheet" href="styles.css">
    </header>


A propriedade rel define a relação entre ambos os arquivos HTML e CSS, já a href define o path que aponta para o nome do arquvo CSS em questão.


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


<h2>Combinando Seletores</h2>


Um seletor CSS pode conter mais de um elemento definido, cirando variações mais específicas de estilização. Por exemplo, é possível definir que apenas elementos children específicos recebam a estilização, sendo chamados de descendant selector:


    <div>
      <p>Selected</p>
      <p>Selected</p>
      <p>Selected</p>
      <a>Unselected</a>
    </div>


Para que apenas um elemento children específico da div seja selecionado, basta declarar deu identificar após o seletor do elemento que o contem, por exemplo:


    div p {
      color: blue;
    }


O mesmo pode ser feito tendo como seletor uma classe, definido uma seleção ainda mais específica. Imagine o seguinte cenário:


    <div class="my-div">
      <h1 class="my-h1">
        Selected
      </h1>
      <h1>
        Unselected
      </h1>
    </div>

    <div>

     ...

    </div>


Para acessar um children específico dentro de uma tag específica, pode-se combinar uma seleção por tag, definindo o tipo de elemento, e por id, definindo qual dos elementos será selecionado:


     div .my-div h1 . my-h1 {
        color: blue;
     }


Além disso, também é possível compartilhar declarações entre elementos definindo mais de um seletor por declaração, separando cada um deles por vírgula:


    .selectorOne {         .selectorTwo {
      font-size: 200%        font-size: 200%
    }                      }


O exemplo acima poderia ser simplesmente:


    .selectorOne, .selectorTwo {
      font-size: 200%
    }


<h2>Declarações</h2>


As declarações são como atributos de um objeto, sendo elas as possibilidades de estilização que podem ser associadas a determinado seletor. Uma declaração consite na junção de propriedade e valor que se separam por dois pontos ```:``` e encerrada por ponto e vírgula ```;```:


<div align="center">
 <img src="https://user-images.githubusercontent.com/61476935/148139655-ffa6ca34-6ac6-4e46-91b1-d55b2e1e6f77.png">
</div>


O CSS conta com mais de [100 propriedades](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) distintas com uma infinidade de valores a serem utilizados. Veremos as mais utilizadas e seus efeitos adiante.


<h1>Box Model</h1>


Uma forma simples de visualizar como o CSS funciona é o conceito de caixas. Uma caisa possui uma série de características que definem um layout, como suas dimensões, podendo ser chamadas de altura e largura, a expessura das laterais que a compõem, o espaço entre as laterais e seu conteúdo, o espaço entre a caixa em si e outros elementos, sua cor e etc. O CSS possui uma propriedade para cada um desses elementos, obviamente não se limitando a estes e muito menos ao formato quadrado de uma caixa.

Para ter uma ideia mais clara sobre o conceito, observe o exemplo a seguir:


<div align="center">
 <img src="https://user-images.githubusercontent.com/61476935/148229865-4e82193d-4658-40bf-9db4-7be410a06a78.png">
</div>


As propriedades descritas no exemplo acima são propriedades básicas e estão presentes em todos os blocos que compõem a estrutura de um template, ou seja, qualquer elemento que fizer parte do DOM pode utilizá-los. Eles definem:


- ```margin```: Consiste na definição de espaço entre um elemento e os demais a sua volta.

- ```padding```: Consiste no espaço entre um elemento e seu conteúdo.

- ```border```: Consiste na expessura, cor e densidade da borda de um elemento.


<h1>Especificações</h1>


Tendo entendido os conceitos básicos do CSS, iremos abordar características mais específicas da estilização de elementos, como as definições básicas de proporção e espaçamento e como utilizá-las, as definições de cores e seus tipos, sombreamento, como atribuir diferentes formas aos elementos, e etc.


<h2>Proporção</h2>


