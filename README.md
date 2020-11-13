# Enxurrada-de-Bits-Exercicios

[![Praticas Enxurrada de Bits](https://img.shields.io/badge/Enxurrada%20de%20Bits-pr%C3%A1ticas-green)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)
[![Enxurrada de Bits - HTML](https://img.shields.io/badge/Enxurrada%20de%20Bits-HTML-red)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)
[![Enxurrada de Bits - CSS](https://img.shields.io/badge/Enxurrada%20de%20Bits-CSS-blue)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)

## Aula 5 

 Nessa prática você irá aprender a:

- [ ] Utilizar loops pra percorrer uma váriavel
- [ ] Adicionar HTML e CSS utilizando Javascript
 
### Novo ponto de aprendizado

Retomando o conteúdo de programação WEB, o que iremos ver aqui nessa prática é uma das formas de aplicação direta de Javacript. Sabemos que javascript, pode se comunicar com a uma página HTML, porém, ainda não aplicamos a linguagem Javascript para modificar diretamente o conteúdo da nossa página HTML. Bom partindo desse ponto, iremos ver aqui como fazer uma alteração no nosso HTML, mas utilizando a mesma "filosofia" de dar continuidade a algo que já está sendo feito. 

**Obs.: Antes de começar essa atividade, tenha em mente que os conhecimentos de loops e funções será necessária, mesmo que de forma mínima**

### Pontos a serem abordados antes da prática


- **Variáveis** : Como já estudamos, variáveis podem conter diferentes tipos de dados, como texto, número inteiro, número irracional, etc. Entretanto, nós não vimos as diferentes maneiras com que os dados podem ser agrupados, e durante essa prática teremos a necessidade de aprender sobre uma das formas de organizar os dados. 
Pois bem, observe o seguinte exemplo:
~~~  
   let nome1 = 'Maria';
   let nome2 = 'Marcus';
   let nome3 = 'Carolina';
   let nome4 = 'João';
   let nome5 = 'Diegão';
~~~
O exemplo acima, nos mostra a declaração de 4 variáveis, as quais são nomes de pessoas, ou seja um texto(string). Bem, imagine que agora eu tenha que ter 150 nomes, logo seguindo a idéia que fizemos acima deveriamos declarar 150 variáveis, mas isso é viável?! Se tivessemos 1000 variáveis, 2000, 3000, isso não iria gerar uma quantidade gigantescas de variáveis?! Então, com o fito de resolver esse problema, o que poderiamos fazer é algo como o exemplo abaixo:
~~~  
   let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
~~~
Bom, no exemplo acima, o que fizemos foi agrupar os dados em uma única variável. Específicamente o que estamos fazendo é uma **Lista**(Array), uma lista é um tipo do javascript que agrupa diferentes tipos de dados, organizados por posições. Pra visualizar essa lista completa podemos simplesmente utilizar o console.log:
~~~  
   let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];    
   console.log(nomes);
~~~
Entretanto, quando utilizamos somente nome da lista, como fizemos no exemplo acima, estaremos utilizando toda a lista. Mas e se eu quiser somente o nome de 'Maria' ?! Então, como foi dito antes, os dados dentro da lista são organizados por posições, e isso permite acessar diferentes posições individualmente. Por exemplo:
~~~  
   let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];    
   console.log(nomes[0]);
   console.log(nomes[3]);
~~~
Observando o exemplo acima, temos uma diferença do que estávamos acostumados, o que estamos fazendo agora é utilizar colchetes '[]' e dentro deles colocarmos um número. Mas o que isso significa?! Bom, quando utilizamos isso, juntamente com o nome da lista, conseguimos acessar as posições individuais da lista. Essas posições começam sempre com 0, vão até a quantidade de elementos - 1 , ou seja no exemplo acima temos 5 elementos na lista, porém as posições dos elementos vão de 0 a 4.  
Caso você execute o exemplo acima, você irá perceber que os nomes 'Maria' e 'João', serão exibido, isso porque são 0 e 3, as respectivas posições dos elementos 'Maria' e 'João'.
**Obs.: Teste os exemplos acima**

- **Loops** e **Lista** : Agora iremos entender como combinar um loop e uma lista, e porque isso é importante. Observe o exemplo abaixo:

~~~  
   let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];    
   console.log(`Nome: ${nomes[0]}`);
   console.log(`Nome: ${nomes[1]}`);
   console.log(`Nome: ${nomes[2]}`);
   console.log(`Nome: ${nomes[3]}`);
~~~

No exemplo acima, fazemos uma interpolação com cada um dos elementos da lista, porém dessa forma caimos no mesmo problema de antes, e se tivessemos 1000 elementos, isso seria viável? Bom, neste ponto é que entram os loops, como temos uma serie de retição que é feita pelo loop, podemos tirar proveito disso. Mas como fazemos isso?! Pois bem,sabemos que um loop deve sempre ter um ponto de início e outro de fim, logo se utilizassemos o exemplo acima, poderíamos fazer um loop que irá rodar de 0 a 3. Entretanto, é bom saber que nem sempre saberemos o tamanho de um lista, pois nem sempre esse valor é estático(fixo), pra resolver esse problema as listas em javascript possuem uma propriedade chamada 'length' que possui o tamanho atual da lista, e que pode ser acessado por 'nomeDaLista.length'. Enfim, levando isso em consideração, podemos então fazer como exemplo abaixo:

~~~  
    let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
    for(let i=0; i< nomes.length; i++){
        console.log(`Nome: ${nomes[i]}`);
    }
~~~

O exemplo acima reduz a quantidade de linhas de código do nosso programa, já que agora não precisamos mais usar nomes[0],nomes [1], nomes [2],nomes[3], pois o i que agora oculpa o espaço entre colchetes '[i]',muda a cada interação do loop.
**Obs.: Teste os exemplos acima**

- **Adicionando HTML e CSS através do Javascript**

Como vimos na última aula, é possível adicionar HTML e CSS através de um código em javascript. Bom,pra aplicar esse conceito e rever o que vimos em aula, vamos primeiro construir o seguinte HTML:

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

.lista{
  color: blue;
}

.sub-lista{
  color: red;
}

~~~

Perceba dentro do corpo da nossa página, temos uma div com um id "caixa", e esse id será de muita importância pra nós.

Pois bem, neste nosso exemplo vamos utilizar duas listas:
~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];
~~~

Essas duas listas irão ser adicionadas ao nosso HTML, de forma que se torne uma lista não ordenada (ul). Pra isso primeiro vamos levar em consideração que as listas são "correspondentes", ou seja 'Maria' é da turma '302', assim como 'Marcus' é da Turma '303', e por aí em diante.

Partindo para parte de adicionar o HTML através do Javascript, vamos utilizar aquela mesma estratégia de loops junto com listas:

~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];

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
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];

 for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
 } 
~~~

Em seguida, vamos criar nosso elemento li:

~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];

 for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
 } 
~~~

Agora vamos criar conteúdo pra o elementoLista, no nosso caso iremos criar um texto, por isso vamos utilizar o método 'createTextNode':

~~~~

 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];

 for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
   let conteudoElementoLista = document.createTextNode(lista[i]);
 } 
~~~~

Depois de criar cada elemento, devemos agora relacioná-los, e nesse caso devemos adicionar o conteudoElementoLista ao elementoLista, e adicionar o elementoLista a lista. Pra isso, vamos utilizar o método appendChild, que adiciona um 'filho' a um elemento:

~~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];

for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
   let conteudoElementoLista = document.createTextNode(nomes[i]);
   
   elementoLista.appendChild(counteudoElementoLista);
   lista.appendChild(elementoLista);
} 
~~~~

Perceba que agora criamos a seguinte estrutura:
~~~~
<ul>
   <li>Maria</li>
</ul>
~~~~

Entretanto, ainda falta a sub lista que devemos adicionar. Pra adicionar ela repetimos o mesmo processo que fizemos com a lista(primeira ul):

~~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];

for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
   let conteudoElementoLista = document.createTextNode(nomes[i]);
   
   elementoLista.appendChild(counteudoElementoLista);
   lista.appendChild(elementoLista);
   
   let subLista = document.createElement('ul'); 
   let elementoSubLista = document.createElement('li'); 
   let conteudoElementoSubLista = document.createTextNode(turmas[i]);
   
   elementoSubLista.appendChild(counteudoElementoSubLista);
   subLista.appendChild(elementoSubLista);
 
} 
~~~~

Perceba que a sub lista foi criada acima, porém ainda não relacionamos a sub lista(segunda ul) com a lista(primeira ul), e é exatamente o que faremos agora:

~~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];

for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
   let conteudoElementoLista = document.createTextNode(nomes[i]);
   
   elementoLista.appendChild(counteudoElementoLista);
   lista.appendChild(elementoLista);
   
   let subLista = document.createElement('ul'); 
   let elementoSubLista = document.createElement('li'); 
   let conteudoElementoSubLista = document.createTextNode(turmas[i]);
   
   elementoSubLista.appendChild(counteudoElementoSubLista);
   subLista.appendChild(elementoSubLista);
   
   lista.appendChild(subLista);
} 
~~~~

Feito isso perceba que a estrutura que desejavamos foi feita, porém, nós ainda não adicionamos essa lista no nosso HTML, isso porque pra isso precisamos inserir os elementos na 
árvore DOM. Bom, recaptulando antes haviamos criado uma div com um id,e é isso que vamos utilizar agora; pra adicionar algo na árvore DOM precisamos de uma referencia, e pra isso criamos a div com um id. Nossa ideia aqui, é adicionar a lista dentro da div, e para isso iremos utilizar dois métodos:

- getElementById : seleciona o elemento com o id passado e retorná-o. (Lembrando que é por esse motivo que não podemos utilizar duas vezes um mesmo id em uma página, já que utilizando esse método, somente um elemento é retornado, ou seja caso haja um outro depois do primeiro retornado, ele é completamente ignorado)

- insertAdjacentElement : Como o proprio nome diz, irá adicionar de forma adjacente a o elemento passado por parâmentro.

**obs: caso não tenha entendido sobre esses métodos, consulte as aulas anteriores**

Bem, com isso em mente vamos então realizar a inserção:

~~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];

for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
   let conteudoElementoLista = document.createTextNode(nomes[i]);
   
   elementoLista.appendChild(counteudoElementoLista);
   lista.appendChild(elementoLista);
   
   let subLista = document.createElement('ul'); 
   let elementoSubLista = document.createElement('li'); 
   let conteudoElementoSubLista = document.createTextNode(turmas[i]);
   
   elementoSubLista.appendChild(counteudoElementoSubLista);
   subLista.appendChild(elementoSubLista);
   
   lista.appendChild(subLista);
   
   document.getElementById('caixa').insertAdjacentElement('beforeend', lista);
} 
~~~~

Agora o que nos falta é adicionar o CSS, para isso vamos fazer o mesmo processo de criar e adicionar algo a o elemento, porém aqui iremos criar um atributo, no nosso caso uma 'class', e depois disso adicionar algo a ele, que no nosso caso é uma das classes que criamos no CSS: 

~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];

for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
   let conteudoElementoLista = document.createTextNode(nomes[i]);
   
   elementoLista.appendChild(counteudoElementoLista);
   lista.appendChild(elementoLista);
   
   let subLista = document.createElement('ul'); 
   let elementoSubLista = document.createElement('li'); 
   let conteudoElementoSubLista = document.createTextNode(turmas[i]);
   
   elementoSubLista.appendChild(counteudoElementoSubLista);
   subLista.appendChild(elementoSubLista);
   
   lista.appendChild(subLista);
   
   let estilo1 = document.createAttribute('class');
   estilo1.value = "lista";
   conteudoElementoLista.setAttributeNode(estilo1);
   
   document.getElementById('caixa').insertAdjacentElement('beforeend', lista);
} 
~~~~

Perceba que criamos um estilo, e setamos o valor dele para uma das classes que criamos no CSS, e por fim adicionamos ela ao conteudoElementoLista, que representa o primeiro 'li' da lista(primeiro ul). 

Bom, agora é só replicar o processo para o conteudoElementoSubLista, criando então um estilo pra ele, atribuindo uma classe a ele, e por fim adicionando de fato o estilo nele:

~~~
 let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
 let turmas = ['302', '303', '305, '303', '304'];

for(let i = 0; i < nomes.length; i++){
   let lista = document.createElement('ul'); 
   let elementoLista = document.createElement('li'); 
   let conteudoElementoLista = document.createTextNode(nomes[i]);
   
   elementoLista.appendChild(counteudoElementoLista);
   lista.appendChild(elementoLista);
   
   let subLista = document.createElement('ul'); 
   let elementoSubLista = document.createElement('li'); 
   let conteudoElementoSubLista = document.createTextNode(turmas[i]);
   
   elementoSubLista.appendChild(counteudoElementoSubLista);
   subLista.appendChild(elementoSubLista);
   
   lista.appendChild(subLista);
   
   let estilo1 = document.createAttribute('class');
   estilo1.value = "lista";
   conteudoElementoLista.setAttributeNode(estilo1);
   
   let estilo2 = document.createAttribute('class');
   estilo1.value = "sub-lista";
   conteudoElementoSubLista.setAttributeNode(estilo2);
   
   document.getElementById('caixa').insertAdjacentElement('beforeend', lista);
 
} 
~~~~

Se você chegou até aqui, e seguiu exatamente os passos anteriores, verá que seu programa ainda não deu certo. Se você abrir seu console, provávelmente verá o seguinte erro:


<p align="center">
   <img src="https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/erroCarregarDOM.png" alt="Foto de Erro ao tentar acessar o ID" />
</p>

Então, esse erro está ocorrendo porque o javascript não conseguiu achar o id que você passou, "uai" mas a gente não criou tudo certinho, porque o javascript não tá achando esse id no DOM? Bem, o motivo desse erro é que o javascript é carregado antes da página toda carregar, ou seja antes da árvore de elementos do DOM, ser preechida por completo, em outras palavras ele não consegue achar o elemento porque ele está procurando antes do tempo. Pra resolver isso, nos utilizamos um evento do javascript chamado onload, que só irá executar quando a 'window' carregar por completo, e esse evento em questão irá executar uma função anônima(sem nome), e dentro dessa função anônima que devemos chamar a fazer nosso algoritmo.

**Obs.: É importante lembrar, que podemos contruir funções fora do window.onload, mas devemos sempre chamá-las dentro da função que irá ser passada pra windown.onload.**  
**Obs.: () => { } é similar a function(){}, ambas são funções anônimas.**


~~~
window.onload = function() {

    let nomes = ['Maria', 'Marcus', 'Carolina', 'João', 'Diegão'];  
    let turmas = ['302', '303', '305, '303', '304'];

   for(let i = 0; i < nomes.length; i++){
      let lista = document.createElement('ul'); 
      let elementoLista = document.createElement('li'); 
      let conteudoElementoLista = document.createTextNode(nomes[i]);

      elementoLista.appendChild(counteudoElementoLista);
      lista.appendChild(elementoLista);

      let subLista = document.createElement('ul'); 
      let elementoSubLista = document.createElement('li'); 
      let conteudoElementoSubLista = document.createTextNode(turmas[i]);

      elementoSubLista.appendChild(counteudoElementoSubLista);
      subLista.appendChild(elementoSubLista);

      lista.appendChild(subLista);

      let estilo1 = document.createAttribute('id');
      estilo1.value = "lista";
      conteudoElementoLista.setAttributeNode(estilo1);

      let estilo2 = document.createAttribute('id');
      estilo1.value = "sub-lista";
      conteudoElementoSubLista.setAttributeNode(estilo2);

      document.getElementById('caixa').insertAdjacentElement('beforeend', lista);

   } 

}
~~~

O resultado deverá ser algo como: 

<p align="center">
   <img src="https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/listaHTMLUsandoJs.png" alt="imagem da lista HTML utilizando javascript" />
</p>

### Começando a alterar o HTML e CSS com Javascript

Bom, como já foi dito é possivél alterar o HTML e o CSS, utilizando Javascript, mas por que isso seria necessário?! Eu não poderia simplesmente alterar diretamente o HTML e o CSS?! Então existem casos em que ficaria quase impossível alterar manualmente certos conteúdos de uma página, seja pelo tamanho , seja pela mudança frequente dos dados. Dito isso, como resolveriamos este problema?! Bem, existem diversas formas, porém a que iremos abordar aqui é mais simples. Porém, antes de começarmos vamos primeiro importar os novos aquivos que iremos precisar:

**Obs.: Não se preocupe, esse aquivos só irão ser utilizados por códigos que serão entregados prontos pra você**
**Obs.: Ignore as partes que estão marcadas de vermelho.

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

Esse arquivo vai tratar de retirar os dados da internet(específicamente do repositorio do github), tratar esses dados, e transformá-los em duas listas, uma que representa os Character(personagens) e outra Description/role(Descrição/Função):

![Programa base atividade](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/programaBaseJSHTMLCSS.png)
          

**Obs: Não se preucupe com as palavras reservadas *'await'* e *'async'*, elas são necessárias pra outra parte do script, com a qual você não irá trabalhar diretamente**

Perceba que as variáveis de lista já foram criadas pra você, a sua missão agora é transformar essas duas listas, em uma lista dentro da outra, como no exemplo onde relembramos como adicionar HTML e CSS com javascript. 


- [X] Utilizar loops pra percorrer uma váriavel
- [X] Adicionar HTML e CSS utilizando Javascript


## FAQ *(perguntas frequentes)*

#### querySelector ?
+ Informações sobre o querySelector </br>
[Link para mais informações](https://pt-br.learnlayout.com/display.html#:~:text=display%20%C3%A9%20a%20propriedade%20mais,%C3%A9%20normalmente%20block%20ou%20inline%20.)


#### Funções anônimas ?
+ Funções anônimas são basicamente funções que podem ser chamadas sem ter a necessidade de ter um nome </br>
[Link para mais informações](https://ricardo-reis.medium.com/fun%C3%A7%C3%B5es-an%C3%B4nimas-javascript-92361075fd89)

#### O que significa windown.onload ?
+ windown é o elemento que representa a janela da nossa página, já onload é o evento que diz quando essa janela foi carregada </br>
[Link para mais informações](https://developer.mozilla.org/pt-BR/docs/Web/API/GlobalEventHandlers/onload)


#### O que são métodos em javascript?
+ [Link para mais informações](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Functions/Definicoes_metodos)

#### O que é um arquivo CSV?
+ [Link para mais informações](https://rockcontent.com/br/blog/csv/)

#### O que é o **Enxurrada de Bits**?
+ Enxurrada de Bits é um projeto de extensão do CEFET-MG, que visa capacitar estudantes de escolas publicas, por meio de cursos de Programação Web, Robótica e Informática Básica. Além de participar e promover eventos, relacionados a área de tecnologia.</br> Saiba mais, pelo [Instagram](https://www.instagram.com/enxurradadebits/?hl=pt-br), e pelo [Site](http://www.enxurradadebits.cefetmg.br/o-enxurrada-de-bits/) do Projeto.


