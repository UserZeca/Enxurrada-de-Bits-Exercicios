# Enxurrada-de-Bits-Exercicios

Olá :) ! Bem vindo(a) as práticas do **Curso de Programação Web**.
Durante essas práticas, você irá desenvolver um projeto, e entender mais de conteúdos abordados na aula.

## Aula 1
 Nessa prática você irá aprender a:

+ Fazer donwload do projeto que está no gitHub (utilizando a interface do site).
+ A organização do projeto
+ Identificar as tags que aprendemos dentro do documento HTML.
+ Inspecionar elementos atráves de ferramentas dos 
navegadores.
+ Utilizar tags ensinadas durante a aula 1.


### Fazendo downloand do projeto

Bom a primeira coisa a se fazer, é baixar o projeto para o seu computador. Pra realizar o download, procure o seguinte botão **Código** (*ou Code, se o idioma do site estiver em inglês*), click em cima deste, e selecione a opção **Download ZIP**.

![Gif mostrando como selecionar o botão de download do repositório](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/downloadRepositorioGitHub.gif)

Como o arquivo está zipado(compactado), será necessário fazer a descompactação(*iremos utilizar o programa gratuito **WINRAR***). Logo quando o download for completado, siga os seguintes passos abaixo:

![Gif mostrando como fazer a descompactação](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/descompactandoProjeto.gif)


### Entendendo a Estrutura do Projeto

Até aqui, o que fizemos foi somente baixar o projeto para a nossa máquina. Mas porque fizemos isso?! Bom, no desenvolvimento de vários projetos nem sempre iremos começá-lo do zero, às vezes teremos que dar continuidade a algo que alguém já foi iniciado, ou fazer alterações pontuais e melhorias. E é exatamente o que iremos fazer aqui.

#### Do que o projeto se trata?
O projeto em sí é uma "mine Wikipedia dos Simpsons", e nela irá conter informações dos 5 integrantes da familia Simpsons. 

![Gif mostrando a página principal do projeto](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/paginaSimpsons.gif)

A página principal, inicialmente está como é mostrado acima, porém ao decorrer das atividades ela será modificada.

*obs.: As páginas do projeto ainda não são resposivas, por motivos didáticos.*

#### Como o projeto foi organizado?

O projeto foi organizado da seguinte forma:

![Foto mostrando a estrutura do projeto, organização de diretórios](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/estruturaBasicaDosArquivos.png)

+ **src** - Pasta(diretório) Raiz que possui todos os codigos, imagens, etc.
+ **componentes** - Pasta(*diretório*) que possui arquivos de estilo relacionados a um elemento especifico da página. ***Não se preocupe com ela, pois ela não é o foco aqui***.
+ **img** - Essa pasta possui as imagens que iremos utilizar para construir as páginas. *obs.: Na maioria das vezes esse pasta fica por padrão dentro de uma pasta chamada asserts, não é o caso aqui.*
+ **paginas** - Dentro dessa pasta termos todas as sub páginas, ou seja todas as páginas que não são a página **home**(principal).
+ **index.html** - Arquivo HTML, que possui o código da página **home**(principal).
+ **styles.css** - Arquivo CSS, que possui todo os estilos da página home. ***Não se preocupe com ele ainda***.


## Identificando, inspecionando e adicionando Tags

Bom, já baixamos o projeto e entendemos sobre a estrutura desse projeto, agora "mão na massa".

+ Abra no navegador o arquivo index.html. Pra fazer isso, vá até a pasta do projeto que baixamos,procure pelo arquivo index.html, e dê um click duplo sobre ele.
Enxurrada-de-Bits-Exercicios-master > src > index.html 

+ Abra o projeto no seu Editor de Código(***Recomendo fortemente o VS Code***), clicando em File > Open Folder .

![Abrindo Projeto](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/abrindoProjeto.gif)

+ Vá até pasta **src**.
+ Selecione o arquivo **index.html**

![Navegando Pelas pastas do projeto](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/NavengadoPelaPastaDoProjeto.gif)

*obs.:Ao abrir esse arquivo, você pode se assutar um pouco com a quantidade de coisa. **Mas calma!** Inicialmente você não irá precisar saber de todo que está no código.*

Enfim, vamos primeiro identificar as tags no código que aprendemos na aula 1 (*não se preocupe com as que **não** estão marcadas em vermelho*):  

![Foto mostrando as tags a serem análizadas](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/Tags1.png)

Aqui podemos identificar as tags que você deverá saber ao estar fazendo essa prática. Ou seja, caso ainda esteja com dúvida de como essas tags funcionam, volte e reveja os materiais referentes a aula. 

*Obs: Perceba a diferença entre a ordem de como os atributos forma colocados na primeira e na segunda tags link(marcadas de vermelho). Bom essa diferença não importa para o seu funcionamento, porém é uma boa prática manter um padrão.*

Agora descendo um pouco mais, avistamos um conjunto grande de tags agrupadas por uma tag chamada ***section***. Por hora vamos ignorar essa parte do código, pois ainda não foi abordado esse conteúdo nas aulas. (porém fica, como desafio, tentar entender pra que serve cada uma destas tags). Caso você esteja utilizando o VS Code ou outro editor editor que também tenha a ferramenta de ocultar partes do código, faça como abaixo. Deixaremos essa parte ocultada, para que seja mais fácil de ler o código.

![Gif mostrando como ocultar parte do código pelo Editor de Códigos VS code](https://github.com/UserZeca/Enxurrada-de-Bits-Exercicios/blob/master/assertsDoReadme/img/Tag2.gif)

Chegando a próxima tag ***section*** podemos ver dentro dela, tags que já conhecemos. Essas tags estão identificadas em vermelho, como mostrado abaixo:

*obs: Não se precupe agora com o que está em amarelo na tag img, e com as tags que ainda não abordamos em aula.*

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

Novamente faremos alterações no código, pórem, agora você verá o resultado final e tentará replicá-lo :



