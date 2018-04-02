# Prova 01 - HTML, SCSS & RWD

## Desenvolvimento de Aplicações Web 

João Eduardo Montandon

Setor de Informática - COLTEC/MG

Valor: 8 pontos

Data: 02/04/2018

## Blog de Tecnologia (8 pontos)

Você foi contratado para desenvolver o protótipo de um blog de tecnologia. Este blog irá cobrir tópicos relacionados a:

*   **Mundo Web:** tópico que conterá notícias relacionadas ao mundo de desenvolvimento web.
*   **Mundo Mobile:** tópico que conterá notícias relacionadas ao mundo de desenvolvimento mobile
*   **eLearning:** tópico que conterá vídeos e tutoriais sobre desenvolvimento web e mobile.

Após discussão com sua equipe, Vocês decidiram dividir o protótipo em quatro partes principais:

*   **Características gerais:** Onde são explicadas as diretrizes gerais do blog.
*   **Página principal:** Onde são explicadas as diretrizes sobre a página principal do blog.
*   **Página do tópico:** Onde são explicadas as diretrizes sobre a página de cada tópico em específico.
*   **Página da notícia:** Onde são explicadas as diretrizes sobre a página de cada notícia do blog.

O documento a seguir irá descrever em detalhes as características de cada parte do protótipo a ser implementado.

### 1.0 - Características gerais

#### Layout

O blog deverá apresentar um layout moderno e clean. Para isso, dê preferência a fundos claros (como branco), e sem cores gradiente. Certifique-se de que o conteúdo da página - assim como seu layout - esteja centralizado (caso a página seja exibida em uma tela superior aos limites definidos pela equipe de design).

<table border="1">
    <tbody>
        <tr>
            <td colspan="2" style="text-slign:center">Resoluções Limites</td>
        </tr>
        <tr>
            <td>Desktop</td>
            <td>1200 pixels</td>
        </tr>
        <tr>
            <td>Tablet</td>
            <td>768 pixels</td>
        </tr>
        <tr>
            <td>Mobile</td>
            <td>560 pixels</td>
        </tr>
    </tbody>
</table>

Para implementação do layout você deverá utilizar, **obrigatóriamente**, um layout híbrido com 16 colunas. Recomenda-se fortemente que tanto o layout híbrido, quanto o restante do estilo sejam feitos utilizando SASS/SCSS.

#### Menu

O menu representa um componente fundamental na navegação do blog. De forma geral, este menu conterá alinhado a esquerda o nome do blog junto de um ícone (40x40). A direita do menu serão exibidos links para acessar os três tópicos do blog.

É importante ressaltar que, assim como todo o blog, o menu deverá ter um comportamento responsivo. Isto é, seu aspecto deverá mudar para se encaixar melhor no dispositivo do usuário. As figuras abaixo mostram como deverá ficar o aspecto do menu nas três resoluções:

<img src="images/menu-m.png">

Além disso, o menu deverá aparecer sempre no topo da página, independentemente da posição vertical na qual o usuário se encontrar.

### 2.0 - Página principal

A página principal, como o próprio nome diz, representa a página inicial do sistema. É por meio desta página que o usuário irá entrar no site. Pensando nisso, sua equipe decidiu fornecer três estruturas de layout: Desktop, Tablet, e mobile.

As figuras abaixo mostram como este site deverá ser organizado para cada layout.



<img src="images/principal-d.png" width="32%"/>
<img src="images/principal-t.png" width="32%"/>
<img src="images/principal-m.png" width="32%"/>

Como pode ser observado, no modelo Desktop a página irá possuir um um container principal, que irá ocupar a largura de toda a página, seguido de três colunas de notícias. O container principal deverá conter uma notícia em destaque, de preferência com uma foto que ocupe todo o container, com o título ao seu lado.

Com relação as colunas, cada uma representa um dos tópicos abordados pelo site. Essas colunas deverão conter as notícias relacionadas aos respectivos tópicos. Além disso, cada tópico deverá ter sua cor específica, similar ao que é feito em portais como [globo.com](http://www.globo.com), [UOL](http://www.uol.com.br), [brainstorm9](http://www.b9.com.br), etc.

As cores poderão ficar a seu cargo. Mas caso ainda não tenha se decidido, segue abaixo uma sugestão (horrível) de cores-base:

*   Web: <span style="background-color: #8AC007; color:white; padding: 0.2em;">#8AC007 ou RGB(138,192,7)</span>
*   Mobile: <span style="background-color: #b51110; color:white; padding: 0.2em;">#b51110 ou RGB(181,17,16)</span>
*   eLearning: <span style="background-color: #2a3744; color:white; padding: 0.2em;">#2a3744 ou RGB(42, 55, 68)</span>

O layout de tablet possui uma estrutura similar ao Desktop, com a diferença de que a coluna de notícias de eLearning foi jogada para baixo, e passou a ocupar a largura de toda a página. Já o layout mobile possui uma estrutura totalmente verticalizada. Cada uma das colunas passa a ocupar um trecho completo da página, sendo empilhadas uma sobre a outra.

#### Fotos

Como diferencial, o dono do blog requisitou que seu site tire o máximo proveito de imagens. Pensando nisso, a equipe de design elaborou a seguinte ideia: Cada notícia conterá uma foto e um título. No entanto, ao passar o mouse sobre a imagem, ela deverá ganhar algum tipo de destaque (ficar escurecida, alterar para preto-e-branco, etc.). Essa ideia foi inspirada no site [brainstorm9](http://www.b9.com.br/).

### 3.0 - Página de um Tópico Específico

As páginas de tópico específico possuirão dois layouts distintos: Desktop e mobile. O Layout de desktop deverá ser aplicado enquanto a largura do browser for superior a 768 pixels. Já o layout mobile deverá ser aplicado para as resoluções de Tablet e Desktop.

<img src="images/topico-d.png" width="65%"/>
<img src="images/topico-m.png" width="34%"/>

No layout Desktop, é importante notar que o conteúdo da página está centralizado, com uma margem considerável entre conteúdo e browser. Ainda, deve-se perceber que, para cada notícia, a mesma deverá ser apresentada com uma foto e seu título lado-a-lado. Ao se passar o mouse em cima da foto, um texto com o subtítulo deverá ser exibido.

Ja no layout mobile, o título da notícia passará a ficar após a foto, e não lado-a-lado (como era no desktop).

Por fim, assim como na página principal, cada tópico deverá ter a cor base definida de acordo com o tópico de interesse. Isto é, as cores da fonte, e outros detalhes do tópico deverão acompanhar a tonalidade escolhida.

### 4.0 - Página da Notícia

A página da notícia foi inspirada no estilo presente no site [medium](http://medium.com). Segue abaixo um protótipo da página de notícias:

[![Noticia](images/noticia-d.png)](images/noticia-d.png)

O título da notícia deverá ser centralizado, com um espaçamento considerável do topo de seu container. O subtítulo por sua vez deverá ter um espaçamento vertical visível a partir do título da página. Ainda, recomenda-se que seja definida uma fonte não serifada para o título da notícia (Trebuchet MS ou Arial, por exemplo).

Além disso, Títulos e subtítulos deverão estar sobre uma imagem de fundo, que irá representar um tópico relacionado a notícia. Essa imagem de fundo deverá ocupar toda a largura do browser, independente da resolução. As [imagens de fundo](http://lorempixel.com/1400/600/) deverão possuir uma proporção de 1400/600\. Ainda, deve-se aplicar um efeito para [escurecer](http://jsfiddle.net/6bjTQ/) as imagens. Como o título da notícia ficará sobre uma imagem escurecida, ambos os elementos (título e subtítulo) deverão definir a cor da fonte como branca. Ainda, o título deverá estar em negrito.


Com relação ao texto da notícia, deverá ser adotada uma fonte serifada (ex: Georgia), e seu tamanho padrão deverá ser de 22 pixels. A primeira letra do primeiro parágrafo deverá receber um estilo personalizado: Seu tamanho deverá ser 3 vezes maior ao tamanho da fonte da notícia.

Além disso, Deverá haver um espaçamento entre os parágrafos equivalente a 1,5 linhas de texto.

## Consulta

Vocês podem consultar **apenas** os materiais abaixo:

* Slides da disciplina
* Seus exercícios
* http://fonts.google.com
* http://fontawesome.io/
* http://www.w3schools.com
* https://color.adobe.com
* https://css-tricks.com/snippets/css/clear-fix/