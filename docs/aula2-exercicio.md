## Aula 2 
 Nessa prática você irá aprender a:

- [ ] Dar continuidade ao projeto
- [ ] Estilizar elementos das nossas páginas 
- [ ] Alterar o HTML e CSS das páginas index.html e bart.html
- [ ] Entender mais sobre o fluxo dos elementos 
- [ ] Entender mais sobre o posicionamento de elementos

### Retomando o que já fizemos

Nos exercícios da aula passada, nós fizemos pequenas alterações no arquivo "index.hmtl" do nosso projeto, e como vimos, esse arquivo representa a página principal do nosso projeto, e em tese ele foi entregue quase pronto para vocês, sendo necessário fazer pequenas alterações. Bom, como vimos durante a segunda aula, há a possibilizade de tornarmos nossa tags menos genéricas, e destravarmos uma limitação, que antes tinhamos ao produzir uma página utlizando somente as tags do HTML.</br>

### Estilizando elementos das nossas páginas

Muitos devem ter percebido, que durante a atividade da última aula, ao adicionarmos links a nossa página, o que estava em negrito, perdeu essa característica e ficou sublinhado e azul.

![Mostrando parte da página com link azul e sublinhado](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoLinkAzul.png)

Vendo isso, muitos devem ter se pensado, o que aconteceu com o estilo em negrito, que eu tinha colocado, e porque o link ficou azul e sublinhado?! Bom, a resposta pra isso tá na caracteristica padrão de todo link no HTML. Por padrão, um link sempre irá adicionar ao texto, as caracteristicas de ser sublinhado e de cor azul. Mas, como vimos na atividade da aula passada, nos não queremos isso. O que fazer para obter o nosso objetivo desejado?! </br>

Então, como dito acima, um link possui caracteristicas visuais padrão, logo o nosso objetivo é "anular" essa caracteristicas. Para isso, iremos primeiro acessar nosso arquivo "styles.css".

<p align="center">
  <img src="https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoArquivoStyles.png" alt="acesando arquivo.styles.css"/>
</p>

Perceba, o que está sublimado de vermelho, é o nosso arquivo. Para seleciona-lo, basta clicar em cima dele (styles.css). *Obs.: caso essa "abinha", não apareça pra você, selecione o icone, representado na imagem acima, circulado de amarelo.* 

Ao abrir o arquivo, podemos ver diversas coisas diferentes.


![Mostrando o Arquivo Styles](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoOArquivoStyles.gif)

Porém o que vamos analizar aqui, são somente o seletores "body", "h1" e "mark".

![Mostrando Seletores do arquivo styles](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoSeletores.png)



Perceba, que na imagem acima, dentro do body podemos ver que há várias propriedades, sendo adiconadas a ele. E essas propriedades alteram o comportamento, posicionamento e estilo do componente, assim como o h1 e mark.

Bom, voltando ao nosso objetivo, o que iremos fazer aqui, é alterar a estilização do nosso link, e para isso o que devemos fazer e adicionar um seletor "a", ao nosso arquivo de estilo. E recaptulando, nos precisamos "anular" o estilo padrão do nosso link. Mas então, como fazemos isso?! No CSS, possui uma propriedade que se chama **text-decoration** (decoração do texto), e ela permite de uma forma mais sucinta, estilizar todo nosso conteúdo de texto, referente ao seletor em que essa propriedade foi colocada. Então, já sabemos o nome da propriedade a ser colocada, mas agora devemos atribuir um valor a ela. O valor passado pra essa propriedade, deve ser **none**, valor esse que quando atribuido a **text-decoration**, irá retirar toda estilização que o link aplicou ao conteúdo de texto dentro dele.</br>

E como dito acima, você deverá:

+ adicionar o seletor **a**;
+ adicionar a propriedade **text-decoration**, dentro do seletor **a**;
+ atribuir **none** a propriedade **text-decoration**;


Após salvar o arquivo "styles.css", recarregue a página "index.html" no seu navegador. Perceba que agora os links, voltaram a estar branco e em negrito:

![Link sem estiização padrão](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/primeiraEdi%C3%A7%C3%A3oDeTexto.png)


### Alterando HTML e CSS das páginas

#### Index

Para finalizarmos por enquanto o trabalho, na página index.html, o que iremos fazer é adicionar links externos para as páginas do Bart e do Homer. Bom, para adicionar esses link devemos primeiro saber onde se localiza as páginas de homer e bart. Na última atividade foi descrito, qual era a estrutura do projeto, e nesse tópico foi dito que há uma pasta chamada "paginas", e nela estão todas as páginas "secundárias" do nosso site. Seu dever agora, e adicionar a cada um dos links, o caminho até esses arquivos. *Obs.: lembre-se o atributo que define o caminho de um link é o **href**, com é mostrado abaixo em vermelho*.

![Mostrando href com caminho pra page Homer](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoHrefComCaminhoPraPageHomer.png)


Agora, ao clicamos na foto do homer ou do bart, somos levados as suas respectivas páginas.


![Mostrando resultado, ao clicar na foto do homer, levando assim a página homer.html](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoComoChegarAPaginaHOmerPelaIndex.gif)


#### Homer

Ao abrir esta página, ou acessando pela pasta ou pelo link na página index, podemos ver uma página com parágrafos, títulos de tamanhos distintos e imagens. 

![Mostrando a Página do Homer](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoP%C3%A1ginaDoHomer.png)

Bom e se você, está se perguntando, porque a página está com estilo parecido com a página index?! Isso,está ocorrendo porque nos exportamos o arquivo styles.css, do nosso projeto, pra dentro da página homer.html:

![Imagem do Head do homer.html, identificando importação de arquivo styles.css](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoImportacaoDoStylesNaPagHomer.png)

E se você já se acostumou em como os elemento aparecem no navegador quando são acionados ao HTML, perceberá que assim como na página index, o fluxo dos elementos não segue o fluxo padrão, que é elemento embaixo de elemento.

Bom, se você pensou na propriedade **float**, neste caso, você acertou! Então, o que está ocorrendo aqui, é que as imagens desta página, receberam a propriedade **float**, e como podemos, uma imagem está a esquerda do texto, e outra a direita.

Enfim, a página homer.html, está ai como um modelo, que iremos adaptar um pouco, para as outras páginas que iremos criar e/ou alterar.

#### Bart

Ao abrir a página Bart, ou pela pasta ou pelo link na página index, podemos ver uma que possui somente um título e um parágrafo, e que como um estilo de letras diferente das outras páginas. Bom, vamos aos poucos, a primeira coisa que devemos fazer ai, é padronizar a nossa fonte com a mesma fonte das outra páginas. E como fazemos isso?! Então, ao exploramos o arquivo styles.css, podemos ver que a fonte declarada ali é ***Balsamiq Sans***, porém essa fonte não é uma fonte que vem por padrão para os documentos HTML,ela, expecificamente neste caso, vem do google fontes, e para adicioná-la a página do bart, devemos referencia-la, adicionando a seguinte tag, dentro do **head** do nosso arquivo bart.html:
~~~
<link href="https://fonts.googleapis.com/css2?family=Balsamiq+Sans&display=swap" rel="stylesheet">
~~~

Feito isso, agora é somente salvar e recarregar a página, que os caracteres irão mudar.

![Página do Bart com os caracteres da forma que queremos, Balsamiq Sans](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoParagrafoComCaracteresCertos.png)

Agora o que iremos fazer e adaptar o modelo do homer aos conhecimentos que já adquirirmos. Bom pra fazer isso você deve copiar o seguinte modelo e adicioná-lo ao seu código.

~~~

 <section>      
      <img src="../../img/" width="25%" height="25%">
    
      <h1>Bart</h1> 
      <p> ... </p>            <!-- Parágrafo 1 (Isso é um comentário, ou seja não intefere no código) -->
      <img src="../../img/">

      <h3>Personalidade</h2>
      <p> ...  </p>         <!-- Parágrafo 2 (Isso é um comentário, ou seja não intefere no código) -->
      <p> ... </p>          <!-- Parágrafo 3 (Isso é um comentário, ou seja não intefere no código) -->

 </section>

~~~

Bom, o que você deverá fazer será o seguinte:

+ Criar uma pasta, chamada bart, dentro da pasta **"img"** do nosso projeto.

+ Baixar duas imagens do Bart Simpson, pra dentro da pasta **bart** que criamos dentro da pasta **img**. *Obs.: O processo pra baixar é o mesmo que baixar uma imagem no google imagens, botão direito > salvar imagem como ...* 
   - [Link para baixar a imagem 1](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/bart1.png)
   - [Link para baixar a imagem 2](github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/bart2.png)

+ Criar um arquivo bartStyles.css dentro da nossa pasta **bart**.
+ Adicionar essa duas imagens dentro de bart.html. *obs.: Perceba que a primeira imagem possui os atributos width e height,que adicionamos porque a imagem bart1 é muito grande, porém você pode alterál-los, se jugar necessário.*
+ O titulo "bart" antigo, ou seja o que não veio com modelo. 
+ Mover o parágrafo antigo, para dentro do primeiro parágrafo dentro da **section**.
+ Adicionar informações da internet, aos parágrafos 2 e 3.


![Página do Bart sem a propriedade float](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoPaginaDoBartSemOStyle.gif)

Ao realizar as tarefas acima, você perceberá que os elemetos não estão alinhados da forma que queremos, já que como no modelo do homer, as nossas fotos deveriam ficar ao lado do noso texto, e não em cima ou embaixo. E porque isso tá acontecendo?! Bom como eu disse, nos iriamos adaptar o modelo seguido no arquivo homer, e como podemos percebe, o código que copiamos e colamos no arquivo bart, não possui muitas coisas que o arquivo homer possui, mas enfim, como eu disse iremos adaptar nosso arquivo bart.

Para isso, a primeira coisa que iremos fazer, será adicionar o atributo **style** a nossa primeira tag **img**. Mas o que esse atributo faz?! Bom, o atributo style, permite adicionar estilos na nossa tag, sem a necessidade de criação de outro arquivo, ou utilização da tag **style** **(ATENÇÂO, SÓ IREMOS FAZER ISSO POR FINS DIDÁTICOS, NÂO É RECOMENDADO UTILIZAR O ATRIBUTO STYLE DIRETAMENTE NA TAG, COMO IREMOS FAZER AQUI)**. Então, sabendo disso, podemos enfim adicionar estilos através do atributo **style**, para fazer isso basta colocar como valor, a propriedade ou as propriedades que queremos adicionar a tag. E como dito antes, o modelo do Homer utiliza a propriedade float para definir o posicionamento dos elementos, e o que iremos fazer aqui é justamente isso.

Para fazer isso, faça como no exemplo abaixo:

~~~  
  <img src="../../img/bart/nomeDasuaImagem1DoBart.algumacoisa"  style="float: left">
~~~

Perceba que o valor de float dentro do atributo style, é left. E relembrando, o que isso significa?! Bom, neste caso a imagem ficará a esquerda do texto:


![Mostrando a primeira foto do bart com a propriedade float com o valor left](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoBartAEsquerda.png)

Bom você deve fazer a mesma coisa com a segunda imagem, mas agora o valor de **float**, será **right**(direita), ou seja "flutuará a direita":

<p align="right">
 <img src="https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/mostrandoBartADireita.png" alt="Mostrando a primeira foto do bart com a propriedade float com o valor right" />
</p>

Perceba agora, que a imagem da nossa página, estará "flutuando", ao lado do texto. Mas, há um problema aqui, a disposição do parágrafo e a distância deles para as fotos, pode ser algo que esteja incomodando. Bom o que você deverá fazer, é:

+ abrir o arquivo bartStyles.css
+ adicionar o seletor de paragrafo. *(dica : seletor p)*
+ adicionar a propriedade de alinhar texto, e defini-la como texto justificado. (caso não lembre, volte nos slides da aula)
+ adicionar o seletor de imagem. *(dica : seletor img)*
+ adicionar uma margin de 15px(pixels).

O resultado final da página bart, deve ser algo parecido com:

![Resultado página do Bart](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/ResultadoPaginaBart.png)

Bom, ao completar essa tarefa, você terá chegado ao fim dessa prática.

- [X] [Deu continuidade ao projeto](retomando-o-que-já-fizemos)
- [X] [Estilizou elementos das páginas](estilizando-elementos-das-nossas-páginas) 
- [X] [Alterou o HTML e CSS das páginas index.html e bart.html](alterando-html-e-css-das-páginas)
- [X] Entendeu mais sobre o fluxo dos elementos 
- [X] Entendeu mais sobre o posicionamento de elementos



## FAQ *(perguntas frequentes)*

#### O que é o **Enxurrada de Bits**?
+ Enxurrada de Bits é um projeto de extensão do CEFET-MG, que visa capacitar estudantes de escolas publicas, por meio de cursos de Programação Web, Robótica e Informática Básica. Além de participar e promover eventos, relacionados a área de tecnologia.</br> Saiba mais, pelo [Instagram](https://www.instagram.com/enxurradadebits/?hl=pt-br), e pelo [Site](http://www.enxurradadebits.cefetmg.br/o-enxurrada-de-bits/) do Projeto.

#### O que é a tag *section*?
+ Para essa prática, não é necessário que você saiba seu funcionamento, mas caso queira saber mais, segue o link:</br>
[Tag section](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/section)

#### O que são **atributos**?
+ Estes conceitos irão ser melhor abordados nas próximas aulas, mas segue o link para mais informações:</br>
[Link para saber mais sobre atributos](https://tableless.github.io/iniciantes/manual/html/oquetags.html)

#### O que é float ?
+ Float é uma propriedade do CSS que permite adicionar flutuações a esquerda ou a direita de elementos, dentro do HTML. </br>
[Link para mais informações](https://medium.com/collabcode/pare-de-chutar-e-aprenda-como-funciona-o-float-left-e-float-right-e-sua-trupe-a4f4161114c7)
