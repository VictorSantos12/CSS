<div align="center">
 <img src="https://user-images.githubusercontent.com/61476935/148092001-97272843-0741-4a7e-8902-f438c3733334.png">
</div>

<br>

<img src="https://img.shields.io/static/v1?label=CSS&message=Style-Sheet&color=blue&style=for-the-badge&logo=CSS"/>


O CSS, ou Cascading Style Sheets, é uma linguagem de folha de estilo utilizada para descrever a indentidade visual de arquivos HTML, XML e entre outros. Sendo uma linguagem padão no desenvolvimento web, o CSS é o responsável pela caracterização estética das páginas web, seguindo uma série de regras definidas pela especificação da W3C para definir cor, estilo de texto, proporcionalidade, formas e tornar a aplicação responsiva.

Tendo sido criado para complementar uma função que era destinada ao HTML, o CSS se tornou tão grande quanto o próprio, estando presente em praticamente qualquer aplicação Web em uma de suas verções, ou estando pré processado em ferramentas como o Sass, Less e Stylus.


<h1>CSS Básico</h1>


Inicialmente, para entender como o CSS se aplica ao HTML, é preciso entender como atrelá-lo a determinado element do DOM. O DOM, ou Document Object Model, é a estrutura que define um Document HTML. Cada tag HTML equivale a um elemento do DOM, sendo renderizado pelo navegador com as caracterésticas a ele atribuidas. O CSS define que um grupo ou determinado elemeto do template será englobado por determinado característica de acordo o conjunto de regras a seguir:


<div align="center">
 <img src="https://user-images.githubusercontent.com/61476935/148107312-1b2b7ed6-95c4-4782-b175-30e3c15f1342.png">
</div>


O chamado <i>conjunto de regras</i> é basicamente um objeto composto pelas seguintes entidades:


<h2>Seletor</h2>


O seletor define o elemento HTML ao qual o style será aplicado, podendo ser definido por classe, por id, por tag e por atributo, sendo declarados da seguinte forma respectivamente:


<h3>Por Classe</h3>


Quando um seletor é definido por classe, todos os elementos DOM que forem declarados com essa classe terão as caracteristicas atribuidas a si. A sintaxe dos seletores definidos por classes é:


    .container {}

    
<h3>Identificador</h3>


Um seletor por identificador, ou id, define que todos os elementos DOM que possuirem determinado id terão as caracteristicas atribuidas a si. A sintaxe dos seletores definidos por id é:


    #menu {}
    

<h3>Por Tag</h3>


Da mesma forma que os anteriores, um seletor definido a partir de determinda tag define que todas as tags do tipo terão as características atribuidas a si.A sintaxe dos seletores definidos por tag é:

    a {}
    

<h3>Por Atributo</h3>


No caso do seletor definido a partir de atributos, todos os elementos DOM do tipo e que possuirem determinado atributo terão as características atribuidas a si. A sintaxe dos seletores definidos por atributo é:


    a[target="_blank"] {}


<h2>Declarações</h2>


As declarações são definidas pelas propriedades do objeto que especificam quais propriedades do elemento serão estilizados, como por exemplo cor, size, font-family e entre outras que serão abordadas posteriormente.


<h2>Propriedades</h2>


As propriedade são as estilizações possíveis de customizar com as regras em determinado elemento.


<h2>Valor</h2>


O valor é definido dentre de uma série de possibilidades disponíveis dentro da regra de estilização do CSS.


