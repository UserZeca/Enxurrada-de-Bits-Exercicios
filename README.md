# Enxurrada-de-Bits-Exercicios

[![Praticas Enxurrada de Bits](https://img.shields.io/badge/Enxurrada%20de%20Bits-pr%C3%A1ticas-green)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)
[![Enxurrada de Bits - HTML](https://img.shields.io/badge/Enxurrada%20de%20Bits-HTML-red)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)
[![Enxurrada de Bits - CSS](https://img.shields.io/badge/Enxurrada%20de%20Bits-CSS-blue)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)

## Aula 5 

 Nessa prática você irá aprender a:

- [ ] Ulilizar loops pra percorrer uma váriavel
- [ ] Adicionar HTML e CSS utilizando Javascript
 
### Novo ponto de aprendizado

Retomando o conteúdo de programação WEB, o que iremos ver aqui nessa prática é uma das formas de aplicação direta de Javacript. Sabemos que javascript, pode se comunicar com a uma página HTML, porém, ainda não aplicamos a linguagem Javascript para modificar diretamente o conteúdo da nossa página HTML. Bom partindo desse ponto, iremos ver aqui como fazer uma alteração no nosso HTML, mas utilizando a mesma "filosofia" de dar continuidade a algo que já está sendo feito. 

**Obs.: Antes de começar essa atividade, tenha em mente que os conhecimentos de loops e funções será necessária, mesmo que de forma mínima**

### Pontos a serem abordados antes da prática


- **Variáveis** : Como já estudamos, variáveis podem conter diferentes tipos de dados, como texto, número inteiro, número irracional, etc. Entretanto, nós não virmos as diferentes maneiras com que os dados podem ser agrupados, e durante essa prática teremos a necessidade de aprender sobre uma das formas de organizar os dados. 
Pois bem, observe o seguinte exemplo:
~~~  
   let nome1 = 'Maria';
   let nome2 = 'Marcus';
   let nome3 = 'Carolina';
   let nome4 = 'João';
~~~
O exemplo acima, nos mostra a declaração de 4 variáveis, as quais são nomes de pessoas, ou seja um texto(string). Bem, imagine que agora eu tenha que ter 150 nomes, logo pelo seguindo a ideia que fizemos acima deveriamos declarar 150 variáveis, mas isso é viável?! Se tivessemos 1000 variáveis, 2000, 3000, isso não iria gerar uma quantidade gigantescas de variáveis?! Então, com o fito de resolver esse problema, o que poderiamos fazer é algo como o exemplo abaixo:
~~~  
   let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];  
~~~
Bom, no exemplo acima, o que fizemos foi agrupar os dados em uma única variável. Específicamente o que estamos fazendo é uma **Lista**(Array), uma lista é um tipo do javascript que agrupa diferentes tipos de dados, organizados por posições. Pra visualizar essa lista completa podemos simplesmente utilizar o console.log:
~~~  
   let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];  
   console.log(nomes);
~~~
Entretanto, quando utilizamos somente nome da lista, como fizemos no exemplo acima, estaremos utilizando toda a lista. Mas e se eu quiser somente o nome de 'Maria' ?! Então, como foi dito antes, os dados dentro da lista são organizados por posições, e isso permite acessar diferentes posições individualmente. Por exemplo:
~~~  
   let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];  
   console.log(nomes[0]);
   console.log(nomes[3]);
~~~
Observando o exemplo acima, temos uma diferença do estavamos acostumados, o que estamos fazendo agora é utilizar colchetes '[]' e dentro deles colocarmos um número. Mas o que isso significa?! Bom, quando utilizamos isso, juntamente com o nome da lista, conseguimos acessar as posições individuais da lista. Essas posições começam sempre com 0, vão até a quantidade de elementos - 1 , ou seja no exemplo acima temos 4 elementos na lista, porém as posições dos elementos vão de 0 a 3.  
Caso você execute o exemplo acima, você ira peceber que os nomes 'Maria' e 'João', serão exibido, isso porque são 0 e 3, as respectivas posições dos elementos 'Maria' e 'João'.
**Obs.: Teste os exemplos acima**

- **Loops** e **Lista** : Agora iremos entender como combinar um loop e uma lista, e porque isso é importante. Observe o exemplo abaixo:

~~~  
   let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];  
   console.log(`Nome: ${nomes[0]}`);
   console.log(`Nome: ${nomes[1]}`);
   console.log(`Nome: ${nomes[2]}`);
   console.log(`Nome: ${nomes[3]}`);
~~~

No exemplo acima, fazemos uma interpolação com cada um dos elementos da lista, porém dessa forma caimos no mesmo problema de antes, e se tivessemos 1000 elementos, isso seria viável? Bom, neste ponto é que entram os loops, como temos uma serie de retição que é feita pelo loop, podemos tirar proveito disso. Mas como fazemos isso?! Pois bem,sabemos que um loop deve sempre ter um ponto de início e outro de fim, logo se utilizassemos o exemplo acima, poderíamos fazer um loop que irá rodar de 0 a 3. Entretanto, é bom saber que nem sempre saberemos o tamanho de um lista, pois nem sempre esse valor é estático(fixo), pra resolver esse problema as listas em javascript possuem uma propriedade chamada 'length' que possui o tamanho atual da lista, e que pode ser acessado por 'nomeDaLista.length'. Enfim, levando isso em consideração, podemos então fazer como exemplo abaixo:

~~~  
    let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];  
    for(let i=0; i< nomes.length; i++){
        console.log(`Nome: ${nomes[i]}`);
    }
~~~

O exemplo acima reduz a quantidade de linhas de código do nosso programa, já que agora não precisamos mais usar nomes[0],nomes [1], nomes [2],nomes[3], pois o i que agora oculpa o espaço entre colchetes '[i]',muda a cada interação do loop.
**Obs.: Teste os exemplos acima**

- **Adicionando HTML e CSS através do Javascript**

Como vimos na última aula, é possível adicionar HTML e CSS através de um código em javascript. Bom,pra aplicar esse conceito e relebramos o que vimos em aula, vamo primeiro contruir o seguinte HTML:

~~~
<!DOCTYPE html>
<html lang="pt">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="stylesheet" href="style.css">
        <title>Página de Teste</title>
    </head>

    <body>
        <div id="caixa">
            <!-- O script irá adicionar "automáticamente" a lista aqui --> 
        </div>
    </body>
</html>
~~~

Em seguida o CSS (com o nome style.css):

~~~

#lista{
  color: blue;
}

#sub-lista{
  color: red;
}

~~~

Perceba dentro do corpo da nossa página, temos uma div com um id "caixa", e esse id será de muita importância pra nós.

Pois bem, neste nosso exemplo vamos utilizar duas listas:
~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];
 let turmas = ['302', '303', '305, '303'];
~~~

Essas duas listas irão ser adicionadas ao nosso HTML, de forma que se torne uma lista não ordenada (ul). Pra isso primeiro vamos levar em consideração que as listas são "correspondentes", ou seja 'Maria' é da turma '302', assim como 'Marcus' é da Turma '303', e por aí em diante.

Partindo para parte de adicionar o HTML através do Javascript, vamos utilizar aquela mesma estratégia de loops junto com listas:

~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];
 let turmas = ['302', '303', '305, '303'];

for(let i = 0; i < nomes.length; i++){
   // O algoritmo virá aqui
}
~~~

Pois bem, a ideia aqui é adicionar uma lista não ordenada dentro da outra, por exemplo:

~~~

<ul>
   <li> Maria </li>
   <ul>
     <li> 302 </li>
   </ul>
</ul>
   
~~~

Perceba que temos uma lista dentro da outra, ou seja a primeira 'ul' terá dois filhos, uma 'li' e uma 'ul', e a partir disso vamos contruir então nosso código. Bom primeiro vamos criar a lista não ordenada(ul), dentro do loop:

~~~
let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];
 let turmas = ['302', '303', '305, '303'];

for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
} 
~~~

Em seguida, vamos criar nosso elemento li:

~~~
let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];
 let turmas = ['302', '303', '305, '303'];

for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
} 
~~~

Agora vamos criar conteúdo pra o elementoLista, no nosso caso iremos criar um texto, por isso vamos utilizar o método 'createTextNode':

~~~~

let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];
 let turmas = ['302', '303', '305, '303'];

for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
   let conteudoElementoLista = document.createTextNode(lista[i]);
} 
~~~~

Depois de criar cada elemento, devemos agora relacioná-los, e nesse caso devemos adicionar o conteudoElementoLista ao elementoLista, e adicionar o elementoLista a lista. Pra isso, vamos utilizar o método appendChild, que adiciona um 'filho' a um elemento:

~~~~

let nomes = ['Maria', 'Marcus', 'Carolina', 'João'];
 let turmas = ['302', '303', '305, '303'];

for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
   let conteudoElementoLista = document.createTextNode(lista[i]);
   
   elementoLista.appendChild(counteudoElementoLista);
   lista.appendChild(elementoLista);
} 
~~~~





### Começando a alterar o HTML e CSS com Javascript

Bom, como já foi dito é possivél alterar o HTML e o CSS, utilizando Javascript, mas por que isso seria necessário?! Eu não poderia simplemente alterar diretamente o HTML e o CSS?! Então existem caso em que ficaria quase impossível alterar manuamente certos conteúdo de uma página, seja pelo tamanho , seja pela mudança frequente dos dados. Dito isso, como resolveriamos este problema?! Bem, existem diversas formas, porém a que iremos abordar aqui é mais simples. Porém, antes de começarmos vamos primeiro importar os novos aquivos que iremos precisar:

**Obs.: Não se preocupe, esse aquivos só irão ser utilizados por códigos que serão estregados prontos pra você**

- Baixe este **[Arquivo1](https://drive.google.com/file/d/10fKyLZIhMg06s11sSgZxPEZcGwxYjDXL/view?usp=sharing)** e adicione a pasta **src** do seu projeto.
- Baixe também este **[Arquivo2](https://drive.google.com/file/d/1mNhPiZ5KrA6CBYjB0EoRvu60wp0PamC5/view?usp=sharing)** e adicione a pasta **src** do seu projeto.
- Adicione o seguinte trecho de código dentro da tag head do Arquivo **index.html**(a página dos simpsons):

~~~
   <script
        src="https://code.jquery.com/jquery-3.5.1.js"
        integrity="sha256-QWo7LDvxbWT2tbbQ97B53yJnYU3WhH/C8ycbRAkjPDc="
        crossorigin="anonymous">
    </script>
    <script src="jquery-csv.js" > </script>
    <script src="https://unpkg.com/axios/dist/axios.min.js"></script>
    <script type="text/javascript" src="index.js"></script>
~~~

Feito isso vamo entender o que iremos fazer. Bom, a ideia aqui é utilizar o Javascript pra adicionar HTML e CSS, de forma que seja realmente vantajoso utilizá-lo ao invés de alterar diretamente, então o que iremos fazer é adicionar uma quantidade relativamente grande no nosso site, porém utilizando javascript. Esses **[dados](https://raw.githubusercontent.com/UserZeca/Enxurrada-de-Bits-Exercicios/master/docs/Characters.csv)** que iremos adicionar, estão na branch master do nosso projeto, e serão capturados por um dos arquivos que você baixou,o index.js. A seguir uma explicação de como o dados estão organizados (**Não se preocupe muito, é só para vocês terem uma ideia**).

#### Arquivo CSV(O arquivo que contém os dados)

Como foi dito, este arquivo está na internet, mas o que este arquivo é?! Bom, basicamente este arquivo possui os dados relacionados aos simpsons que iremos utilizar. Esse arquivo é do tipo CSV, um tipo de arquivo muito usado em análise de dados, e intepretando este arquivo podemos ver que os dados ficam organizados da seguinte forma:

~~~
        Character    |   Description/role
      Homer Simpson     father of Bart, Lisa, and Maggie
      Marge Simpson     Wife of Homer; mother of Bart, Lisa, and Maggie
      Bart Simpson      Oldest child and only son of Homer and Marge; brother of Lisa and Maggie
      ...               ...
~~~
**obs.: Omitir o restante das colunas, pois ela não serão utilizadas**

Bom, acima podemos ver que os arquivos csv são organizados de forma similar a uma tabela e exatamente esse conceito que será levado em consideração para o nosso algoritmo.

#### Arquivo index.js

Esse arquivo vai tratar 




- [X] Dar continuidade ao projeto
- [X] Utilizar class e id 
- [X] Aprender a colocar um vídeo na sua página 
- [X] Criar o restante das páginas, ou seja a dos outros personagens



## FAQ *(perguntas frequentes)*

#### O que é display ?
+ Display é uma das propriedades mais importante que possuimos no css, já que ela controla o layout da nossa página html. </br>
[Link para mais informações](https://pt-br.learnlayout.com/display.html#:~:text=display%20%C3%A9%20a%20propriedade%20mais,%C3%A9%20normalmente%20block%20ou%20inline%20.)


#### O que é display flex ?
+ Display flex, é uma propriedade, utilizada pra modificar o comportamento de elementos da nossa página. </br>
[Link para mais informações](https://origamid.com/projetos/flexbox-guia-completo/)

#### O que é iframe ?
+ Tag utilizada para adicionar conteúdos de outras páginas/sites.</br>
[Link para mais informações](https://www.hostinger.com.br/tutoriais/o-que-e-iframe/)


#### O que é a tag *section*?
+ Para essa prática, não é necessário que você saiba seu funcionamento, mas caso queira saber mais, segue o link:</br>
[Tag section](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/section)

#### O que são **atributos**?
+ Estes conceitos irão ser melhor abordados nas próximas aulas, mas segue o link para mais informações:</br>
[Link para saber mais sobre atributos](https://tableless.github.io/iniciantes/manual/html/oquetags.html)

#### O que é o **Enxurrada de Bits**?
+ Enxurrada de Bits é um projeto de extensão do CEFET-MG, que visa capacitar estudantes de escolas publicas, por meio de cursos de Programação Web, Robótica e Informática Básica. Além de participar e promover eventos, relacionados a área de tecnologia.</br> Saiba mais, pelo [Instagram](https://www.instagram.com/enxurradadebits/?hl=pt-br), e pelo [Site](http://www.enxurradadebits.cefetmg.br/o-enxurrada-de-bits/) do Projeto.


