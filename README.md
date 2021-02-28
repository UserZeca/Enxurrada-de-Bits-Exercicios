# Enxurrada-de-Bits-Exercicios
[![Praticas Enxurrada de Bits](https://img.shields.io/badge/Enxurrada%20de%20Bits-pr%C3%A1ticas-green)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)
[![Enxurrada de Bits - HTML](https://img.shields.io/badge/Enxurrada%20de%20Bits-HTML-red)](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/edit/master/README.md)

## Aula 1 

Nessa prática você irá aprender a:

- [ ] [Fazer donwload do projeto que está no gitHub (utilizando a interface do site)](#fazendo-downloand-do-projeto).
- [ ] [A organização do projeto](#entendendo-a-estrutura-do-projeto)
- [ ] [Identificar as tags que aprendemos.](#identificando-inspecionando-e-adicionando-tags)
- [ ] [Inspecionar elementos através de ferramentas dos 
navegadores.](#identificando-inspecionando-e-adicionando-tags)
- [ ] [Utilizar tags ensinadas durante a aula 1.](#identificando-inspecionando-e-adicionando-tags)

### Fazendo downloand do projeto

Bom a primeira coisa a se fazer, é baixar o projeto para o seu computador. Pra realizar o download, procure o seguinte botão **Código** (*ou Code, se o idioma do site estiver em inglês*), click em cima deste, e selecione a opção **Download ZIP**.

![Gif mostrando como selecionar o botão de download do repositório](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/downloadRepositorioGitHub.gif)

Como o arquivo está zipado(compactado), será necessário fazer a descompactação (iremos utilizar o programa gratuito [***WINRAR***](#eu-não-tenho-o-winrar-como-faço-pra-baixá-lo) ). Logo quando o download for completado, siga os seguintes passos abaixo:

![Gif mostrando como fazer a descompactação](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/descompactandoProjeto.gif)


### Entendendo a Estrutura do Projeto

Até aqui, o que fizemos foi somente baixar o projeto para a nossa máquina. Mas porque fizemos isso?! Bom, no desenvolvimento de vários projetos nem sempre iremos começá-lo do zero, às vezes teremos que dar continuidade a algo que alguém já foi iniciado, ou fazer alterações pontuais e melhorias. E é exatamente o que iremos fazer aqui.

#### Do que o projeto se trata?
O projeto em sí é uma "mine Wikipedia dos Simpsons", e nela irá conter informações dos 5 integrantes da familia Simpsons. 

![Gif mostrando a página principal do projeto](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/paginaSimpsons.gif)

A página principal, inicialmente está como é mostrado acima, porém ao decorrer das atividades ela será modificada.

*obs.: As páginas do projeto ainda não são [resposivas](#faq-perguntas-frequentes), por motivos didáticos.*

#### Como o projeto foi organizado?

O projeto foi organizado da seguinte forma:

![Foto mostrando a estrutura do projeto, organização de diretórios](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/estruturaBasicaDosArquivos.png)

+ **src** - Pasta(diretório) Raiz que possui todos os códigos, imagens, etc.
+ **componentes** - Pasta(*diretório*) que possui arquivos de estilo relacionados a um elemento especifico da página. ***Não se preocupe com ela, pois ela não é o foco aqui***.
+ **img** - Essa pasta possui as imagens que iremos utilizar para construir as páginas. *obs.: Na maioria das vezes esse pasta fica por padrão dentro de uma pasta chamada asserts, não é o caso aqui.*
+ **paginas** - Dentro dessa pasta termos todas as sub páginas, ou seja todas as páginas que não são a página **home**(principal).
+ **index.html** - Arquivo HTML, que possui o código da página **home**(principal).
+ **styles.css** - Arquivo CSS, que possui todo os estilos da página home. ***Não se preocupe com ele ainda***.


## Identificando, inspecionando e adicionando Tags

Bom, já baixamos o projeto e entendemos sobre a estrutura desse projeto, agora "mão na massa".

+ Abra no navegador o arquivo index.html. Pra fazer isso, vá até a pasta do projeto que baixamos,procure pelo arquivo index.html, e dê um click duplo sobre ele.
Enxurrada-de-Bits-Exercicios-master > src > index.html 

+ Abra o projeto no seu Editor de Código(***Recomendo fortemente o [VS Code](#faq-perguntas-frequentes)***), clicando em File(arquivo) > Open Folder(abrir pasta) .

![Abrindo Projeto](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/abrindoProjeto.gif)

+ Vá até pasta **src**.
+ Selecione o arquivo **index.html**

![Navegando Pelas pastas do projeto](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/NavengadoPelaPastaDoProjeto.gif)

*obs.:Ao abrir esse arquivo, você pode se assustar um pouco com a quantidade de coisa. **Mas calma!** Inicialmente você não irá precisar saber de todo que está no código.*

Enfim, vamos primeiro identificar as tags no código que aprendemos na aula 1 (*não se preocupe com as que **não** estão marcadas em vermelho*):  

![Foto mostrando as tags a serem análizadas](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/Tags1.png)

Aqui podemos identificar as tags que você deverá saber ao estar fazendo essa prática. Ou seja, caso ainda esteja com dúvida de como essas tags funcionam, volte e reveja os materiais referentes a aula. 

*Obs: Perceba a diferença entre a ordem de como os [atributos](#o-que-são-atributos) forma colocados na primeira e na segunda tags link(marcadas de vermelho). Bom essa diferença não importa para o seu funcionamento, porém é uma boa prática manter um padrão.*

Agora, descendo um pouco mais, avistamos um conjunto grande de tags agrupadas por uma tag chamada [**section**](#o-que-é-a-tag-section). Por hora vamos ignorar essa parte do código, pois ainda não foi abordado esse conteúdo nas aulas. (porém fica, como desafio, tentar entender pra que serve cada uma destas tags). Caso você esteja utilizando o VS Code ou outro editor que também tenha a ferramenta de ocultar partes do código, faça como abaixo. Deixaremos essa parte ocultada, para que seja mais fácil de ler o código.

![Gif mostrando como ocultar parte do código pelo Editor de Códigos VS code](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/Tag2.gif)

Chegando a próxima tag [**section**](#o-que-é-a-tag-section) podemos ver dentro dela, tags que já conhecemos. Essas tags estão identificadas em vermelho, como mostrado abaixo:

*obs: Não se preocupe agora com o que está em amarelo na tag img, e com as tags que ainda não abordamos em aula.*

![Segunda Section do projeto](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/Tags3.png)

Agora iremos fazer pequenas alterações nesse trecho de código. 
+ Identifique a tag de parágrafo
+ Deixe o fundo nome do criador do Simpsons, "Matt Groening", destacado. (*Dica: use a tag **mark***) 
+ Deixe as seguintes partes do texto em negrito: (*Dica: use a tag **strong***)
    - "Homer"
    - "Marge"
    - "Bart"
    - "Lisa"
    - "Maggie"
+ Vá até a página index.html,aberta anteoriormente no navegador, e recarregue a página. (*Dica: utilize a tecla **F5***)

***obs: Não se esqueça de salvar as mudanças do seu projeto, "control+s" é sempre seu amigo :).***

O resultado deve ser algo como:

![Primeira Edição De Texto](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/primeiraEdi%C3%A7%C3%A3oDeTexto.png)


Feito isso vamos a próxima parte do código. Aqui, você deverá saber o que são as tags marcadas de vermelho.

*Obs.: O que está de amarelo, deve ser ignorado por enquanto.*

![Parte do código, terceira section do arquivo index ](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/SegundaSectionDoIndex.png)

Agora você irá realizar alterações no código, vendo o resultado final, assim tentar replicá-lo :

![Segunda Edição de Texto](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/segundaEdi%C3%A7%C3%A3oDeTexto.png)

Na próxima *[**section**](#o-que-é-a-tag-section)* você irá identificar as tag necessárias, modificar seu conteúdo, para que o resultado seja o seguinte:

![Terceira Edição de Texto](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/TerceiraEdi%C3%A7%C3%A3oDeTexto.png)

A última [**section**](#o-que-é-a-tag-section) desse arquivo, possui imagens do personagens principais, e cada uma dessas imagens também é um link. Mas como assim um link?! Bom, o que está acontencendo é que o conteúdo dentro da **a** , no caso é uma imagem, está recebendo as caracteristicas da [**tag pai**](#o-que-você-quis-dizer-com-tag-pai), que é justamente a tag **a**.

![Link na imagem,código](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/linkNaImagemCode.png)

Bom, sua missão agora é adicionar um **[link interno](#faq-perguntas-frequentes)**, a cada uma dessas fotos. Volte na **primeira tag de parágrafo** do site, e coloque os links internos no nome de cada personagem (inclusive já colocamos estes nomes em negrito, anteriormente). *E lembre-se, o atributo [**href**](#o-que-significa-href) nesse caso, deve ser ( #atributo name do seu link destino). Por exemplo, na imagem acima o [atributo](#o-que-são-atributos) name do link destino é **homer**, logo o link de ponto de partida deve ter o atributo href="#homer"*.

O resultado deve ser algo como:
![Resultado de adicões de links internos a página](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/VisualizandoLinkInterno.gif)

Por último, iremos visualizar as nossas mundaças, utilizando ferramentas de desenvolvimento que os navegadores possuem.
Para abrir a ferramenta pressione:

+ F12, caso esteja usando o **Google Chrome**
+ Ctrl + Shift + K, caso esteja usando o **FireFox**

Feito isso, o navegador irá abrir uma um caixa de funcionalidades. *obs.: As ferramentas dos dois navegadores são bem parecidas.*

![Mostrando Ferramentas do Navegador](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/MostrandoFerramentaDeDesenvolvedor.png)

Perceba que a parte que está dentro do quadrado vermelho, são as [**section**](#o-que-é-a-tag-section) do nosso código, e que a circulada em verde foi a primeira que alteramos nessa prática.
Os navegadores possuem também, uma ferramenta que permite inspecionar elementos. Pra utiliza-la, faça como a demostração abaixo:

![Mostrando como se utiliza o Inspetor de elementos do navegador](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/MostrandoOInspetordeElementos.gif)

+ Observe que ao passar o mouse por cima de uma parte do codigo na aba **Elements** a parte em que estamos com o mouse em cima fica azul, assim como a sua respectiva parte na nossa página. 
+ Acima também podemos ver que ao selecionarmos a ferramenta de inspecionar(a com icone de setinha em cima de uma quadrado), temos a liberdade de selecionar qualquer elemento da tela, clicando nele. No exemplo acima, podemos ver que ao selecionarmos o nome de Matt Groening(com inspetor acionado), a aba de **Elements** se atualiza, e podemos ver como aquilo aparece no nosso código, além disso ao passarmos o mouse sobre qualquer elemento, podemos ver suas caractéristica, como cor, cor de fundo, tipo de fonte, etc.

Enfim, você chegou ao final da primeira prática.

- [X] [Download do projeto que está no gitHub (utilizando a interface do site).](#fazendo-downloand-do-projeto)
- [X] [Entendeu a organização do projeto.](#entendendo-a-estrutura-do-projeto)
- [X] [Identificou as tags que aprendemos.](#identificando-inspecionando-e-adicionando-tags)
- [X] [Inspecionou elementos atráves de ferramentas dos 
navegadores.](#identificando-inspecionando-e-adicionando-tags)
- [X] [Utilizou tags ensinadas durante a aula 1.](#identificando-inspecionando-e-adicionando-tags)


## FAQ *(perguntas frequentes)*

#### O que é o **Enxurrada de Bits**?
+ Enxurrada de Bits é um projeto de extensão do CEFET-MG, que visa capacitar estudantes de escolas publicas, por meio de cursos de Programação Web, Robótica e Informática Básica. Além de participar e promover eventos, relacionados a área de tecnologia.</br> Saiba mais, pelo [Instagram](https://www.instagram.com/enxurradadebits/?hl=pt-br), e pelo [Site](http://www.enxurradadebits.cefetmg.br/o-enxurrada-de-bits/) do Projeto.

#### O que são **links internos** ? 
+ Um link interno é uma forma de fazer com que um link aponte pra dentro da própria página, como um sumário cheio de tópicos, que ao selecionarmos um desses tópicos, somos redirecionados a parte do texto que trata daquele tópico em questão. Exemplo, o próprio sumário desse documento, possui links internos. </br>
[Link para mais informações](https://www.alura.com.br/artigos/ancorando-elementos-com-html5)

####  O que é um site reponsivo ?
+ Um site reponsivo, é um site que adapte seu layout(seu modelo gráfico de site), a diversos tamanhos de tela:</br>
[Link para mais informações](https://www.agenciakaizen.com.br/desenvolvimento-de-sites/o-que-e-um-site-responsivo/)

#### Eu não tenho o **Winrar**, como faço pra baixá-lo?
+ O link abaixo irá levá-lo a página oficial do software, lá você poderá baixá-lo pra versão do seu sistema operacional, gratuitamente (free):</br>
[Link para baixar o Winrar](https://www.win-rar.com/start.html?&L=9)

#### Como baixar o VS Code ?
+ O link abaixo irá levá-lo a página oficial do software, lá você poderá baixá-lo pra versão do seu sistema operacional, gratuitamente (free):</br>
[Link para baixar o VS Code](https://code.visualstudio.com/download)

#### O que é a tag *section*?
+ Para essa prática, não é necessário que você saiba seu funcionamento, mas caso queira saber mais, segue o link:</br>
[Tag section](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/section)

#### O que são **atributos**?
+ Estes conceitos irão ser melhor abordados nas próximas aulas, mas segue o link para mais informações:</br>
[Link para saber mais sobre atributos](https://tableless.github.io/iniciantes/manual/html/oquetags.html)

#### O que você quis dizer com "tag pai"?
+ Esse conceito está ligado a forma de como os elementos são estruturados no documento html, para saber mais segue o link:</br>
[Hieraquia HTML](https://wtricks.com.br/hierarquia-no-html/)

#### O que significa "*href*"?
+ Href é a abreviatura de Hypertext Reference, atributo de um documento HTML, que define um vínculo com outro documento da Web. Para mais informações, segue o link abaixo:</br>
[Contextualização do que é o atributo href](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/a)
