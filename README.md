# Enxurrada-de-Bits-Exercicios

[![Praticas Enxurrada de Bits](https://img.shields.io/badge/Enxurrada%20de%20Bits-pr%C3%A1ticas-green)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)
[![Enxurrada de Bits - HTML](https://img.shields.io/badge/Enxurrada%20de%20Bits-HTML-red)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)
[![Enxurrada de Bits - CSS](https://img.shields.io/badge/Enxurrada%20de%20Bits-CSS-blue)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)

## Aula 4 

 Nessa prática você irá aprender a:

- [ ] Dar continuidade ao projeto
- [ ] Utilizar class e id 
- [ ] Aprender a colocar um vídeo na sua página 
- [ ] Criar o restante das páginas, ou seja a dos outros personagens




### Retomando o que já fizemos

Nos exercícios da aula passada, nós fizemos pequenas alterações no arquivo "bart.html" do nosso projeto, e como vimos, esse arquivo representa a página do Bart no nosso projeto, e em tese ele foi entregue quase pronto para vocês, sendo necessário fazer alterações. Bom, como vimos durante a segunda aula, há a possibilidade de tornarmos nossa tags menos genéricas, e destravarmos uma limitação, que antes tinhamos ao produzir uma página utlizando somente as tags do HTML. Pórem, depois da aula 4 aprendemos que as tags podem se tornar exclusivas, mesmo sendo do mesmo tipo.</br>

**Antes de começar essa atividade, adicione a propriedade "display: flex;", dentro do seletor "p", no arquivo de estilo do bart. Essa propridade, neste caso, fará com que o texto se encaixe melhor entre as imagens.

### Utilizando class e id

Muitos devem ter percebido, que durante a atividade da última aula, utilizamos a tag style, para diferenciar nosso elementos. Pórem, agora com os conhecimentos que temos, não precisamos fazer mais isso. Bom, o que iremos fazer é substituir os styles, por uma classes que irão fazer a mesma coisa, porém, agora o código ficará de forma mais organizada e fácil de alterar(se necessário). Essas classes, pórem, já existem desde a criação do projeto, elas estão dentro do nosso arquivo style.css. 

![Imagem do styles.css](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/img3.png)

Como já estamos importando as classes do arquivo styles.css, sua missão agora, é identificar qual classe substituirá cada atributo style, e assim alterar o arquivo do bart.html</br>

#### Adicionando um vídeo a página

Bom, o que iremos fazer agora é adicionar um vídeo qualquer, sobre o bart. Pra isso iremos utilizar a tag **iframe**, essa tag incorpora um conteúdo de um site externo ao seu, e é exatamente o que iremos fazer. <br>

Pesquise no Youtube, por qualquer vídeo sobre "Bart Simpsons".

![mostando como pegar iframe no Youtube](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/MostrandoComoPegarIframeNoYoutube.gif)

Logo após, faça como a demostração acima, copie a tag que o youtube já te entrega pronta, e coloque entre uma **nova section**, por exemplo:

~~~

  ... 
   <section>
     
     Coloque a tag iframe aqui!
   
   </section>
  ...

~~~

Perceba, que agora há um vídeo na sua página, porém ele está posicionado de uma forma que não queremos. O que vamos fazer é deixá-lo centralizado. Pra fazer isso utilizaremos a display flex (a partir de agora é importante, que vocês aprendam um pouco sobre essa propriedade, veja mais em **[faq](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/aula4-exercicios/README.md#faq-perguntas-frequentes)**), essa propriedade, irá mudar o comportamento do nosso elemento, permitindo que possamos utilizar novas propriedades pra realizar o alinhamento. Pois bem, adicione uma class, chamada "alinharAoCentro", e coloque dentro do escopo da tag **section**:

~~~  
   <section class="alinharAoCentro">
     <iframe  ...... >

     </iframe>
  </section>   
  
~~~

Agora dentro do arquivo de CSS do bart, crie uma **class**, com o mesmo nome que acionamos a classe, anteriormente, dentro do escopo da tag section. Agora, dentro dele adicione as seguintes propriedades:

~~~
  .alinharAoCentro{
    display: flex;
    justify-content: center;
  }
~~~

A propriedade display, irá mudar o comportamento geral do elemento, e a propriedade justify-content, permitirá alinhar o elemento na horizontal, neste caso, ao centro.<br>
Feito isso, perceba que ele talvez ele ainda não esteja na posição que você deseja. Tente posicioná-lo, utilizando propriedades que já vimos nas aulas anteriores.

Agora, vamos utilizar um id, pra personalizar um pouco nosso iframe. Adicione um **id**, chamado vídeo e coloque dentro do escopo da tag **iframe**. Depois disso, vá até o arquivo de CSS do bart, e crie um id, como o mesmo nome do id adicionado dentro do iframe. Neste ponto, o que você deve fazer é utilizar sua criativide, talvez acionar uma borda, uma cor de fundo, mas tente estilizar o iframe. 

Por fim sua página do bart, deve estar similar a página abaixo:

![Mostrando página do Bart com vídeo, utilizando Iframe](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/MostrandoPaginaDoBartComVideo.gif)



### Criar o restante das páginas, ou seja a dos outros personagens

A partir desse ponto, as atividades de cada um irão se diferenciar tanto na criatividade, quanto na aplicação. Porém, você deverá segui mais ou menos o mesmo modelo das páginas anteriores. Bom, o que você deverá fazer daqui pra frente, é utilizar todos os padrões e conteúdos aprendidos durante as duas outras práticas, e fazer as páginas dos demais personagens, Maggie, Lisa e Marge. Lembrando, que após terminar, você deverá adicionar os links pras essas páginas, dentro daquela seção de links que alteramos lá na prática 1 (a das fotinhas dos personagens).

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


