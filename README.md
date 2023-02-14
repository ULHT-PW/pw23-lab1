**UNIVERSIDADE LUSÓFONA**

# Programação Web - Laboratório 1: <br>*O meu primeiro website*

## Objetivo:
* Neste laboratório criará um website sobre uma cidade à sua escolha, onde irá aplicar os conceitos aprendidos sobre HTML adquiridos esta semana.
* Este laboratório deverá ser concluido antes da sua aula prática da semana de 20.2, onde será avaliado. 

## Recomendações
* Leia o enunciado todo com atenção antes de o começar a resolver para entender o que fará.
* Execute com atenção cada passo, certificando-se que implementa todos os detalhes. Contém todos os detalhes para a criação do website. 
* Se tiver alguma dúvida, recorra aos slides da aula que contêm todos os conhecimentos que precisa para realizar o laboratório.

## Pré-requisitos
* Deverá ter o VS Code instalado para editar o código HTML de forma fácil.
* Instale no VS Code a extensão live server
* Para que fique bem indentado, utilize o comando Shift+Alt+F


# HTML

O HTML é uma linguagem de marcação para construir páginas Web. OS ficheiros HTML possuem marcadores (*tags*), palavras entre parênteses angulares (`<` e `>`) que são comandos de formação da linguagem. 

Reveja se necessário os slides apresentados nos [slides da aula prática](https://github.com/ULHT-PW/pw23-lab1/files/10727143/pw-lab1.pdf)

No elemento `<title>Primeira página</title>`:
* `<title>` é o marcador de abertura
* `</title>` é o marcador de fecho
* `Primeira página` será o conteúdo afetado pelo marcador <title>, que neste caso especificará o título da barra de navegação.

No ficheiro em cima poderá ver a utilização de vários marcadores:
* `h1` = marcador que define um titulo - heading1 (`h2` um subtítulo, `h3` um subsubtítulo, ...)
* `p` = marcador que define um parágrafo
* `ul` = marcador que define uma lista não numerada (`ol` para lista numerada)
* `li` = marcador que define uma linha
* `img` = marcador que define uma imagem
* `a` = marcador de âncora para hiperlink, especificado como valor do atributo `href` 

Dentro de um marcador podem ser especificados pares de atributo = valor. Os atributos modificam os resultados padrões dos elementos e os valores caracterizam essa mudança. Existem neste ficheiro os seguintes atributos:
* `src` = atributo que define o nome do ficheiro com a imagem
* `href`= atributo que define o URL da hiperligação
Nas próximas aulas falaremos mais em detalhe destes aspectos.


# Página Web 

Fará neste laboratório um website sobre uma cidade do mundo à sua escolha que goste. Deverá congregar várias informações sobre esta conforme indicado ao longo do laboratório. 

1. crie uma pasta `lab1` e abra-a com o VSCode.  

2. crie o ficheiro `index.html`, inserindo as seguintes partes elementares de um ficheiro HTML:

```html
<!DOCTYPE html>
<html lang="pt">
    <head>
    </head>
    <body>
    </body>
</html>
```

1. Na secção <head> insirta os seguintes elementos (veja os slides da aula!):
    1. ESpecifique como título da barra do navegador (etiqueta <title>) o nome da sua cidade. 
    2. Especifique também os seguintes metadados:
        1. codificação UTF-8 (para poder visualizar emojis e carateres não ASCII tipo ç, ã, õ). 
        2. nome do autor do site, descrição do conteudo do site, e palavras chave: 
            * `<meta name="author" content="Ana Maria">`
            * `<meta name="keywords" content="palavras chave">`
            * `<meta name="description" content="Website sobre Lisboa">`

# A minha primeira página

Crie agora a sua primeira página. Siga o template em baixo. Terá o nome da Cidade, uma imagem e o menu, ficando da seguinte forma:

![cabecalho](https://user-images.githubusercontent.com/42048382/218595546-59a5863a-0f14-4002-8176-80d2ae3b2aa2.png)

Para, tal, siga os seguintes passos (reveja os slides da aula prática): 
1.	No body, insira um elemento `h1` com o nome da cidade.
2.	Na linha seguinte insira uma imagem da cidade a seu gosto. Redimensione a imagem para que tenha 300px de largura.No Paint existe uma opção resize que lhe permite escolher o número de pixels que pretende que tenha de largura. Respeite a proporção da imagem, sem a deformar! Guarde a imagem numa nova pasta `images`. Insira a imagem usando a etiqueta `img`. 
3.	Deverá inserir, depois da imagem, uma quebra de linha, `br`, pois o elemento `img` não introduz uma quebra.

4. Insira um titulo `h2` com a palavra Introdução 
5. Finalmente, escreva uma frase sobre a cidade.

    
A sua página está pronta!   
1. visualize a sua pagina, clicando diretamente no ficheiro HTML na pasta. O seu browser abrirá e renderizará a página.
2. visualize a sua pagina, clicando no canto inferionr direito em "Go live". Deixe sempre aberto. Todas as alterações que for  fazendo serão automaticamente refrescadas.


# Mais páginas para o meu website!

Irá agora criar várias páginas interligadas, como no slide da aula prática. Reveja os [slides 15 e 16](https://github.com/ULHT-PW/pw23-lab1/files/10727143/pw-lab1.pdf) PAra tal:
1. Crie o menu. Para tal:
    1. Crie cinco etiquetas de hiperlink `a`, tendo como conteúdo o nome das páginas do seu site (Introdução, Localização, Multimédia, Informações, Home), estando os elementos separados pelo carater `|`. 
    2. Use como valor para o atributo `href` as seguintes páginas:
        1. `index.html` para Introdução 
        2. `local.html` para Localização
        3. `multimedia.html` para Multimédia
        4. `info.html` para Informações

3.	Crie 4 copias do ficheiro index.html que criou. 
4.	Altere os nomes dos ficheiros para ter um de cada, com os seguintes nomes: index.html, local.html, multimedia.html, info.html (atenção que os nomes dos ficheiros HTML  deverão estar em minúsculas, sem espaços, acentos ou carateres especiais)
5.	Em cada ficheiro, no menu ponha a negrito a palavra a que corresponde a página. PAra pôr a negrito colocque a etiqueta `b`em volta do hiperlink devido.
6.	Abra o ficheiro index, e experimente se os hiperlinks funcionam. 
Tem agora criado o seu website! Agora irá preencher cada página com conteúdos.

# Página Introdução

Na pagina `index.html` insira, no body, por debaixo da frase que escreveu sobre a cidade crie:
3. Pequena história divertida:  
    1. Conte uma pequena história divertida apenas com emojis 😉, sobre a :cityscape: que escolheu. Explore emojis, premindo nas teclas `🙂Windows + .`, ou pesquise na Internet em [emojipedia](https://emojipedia.org/), [carateres especiais UTF-8](https://www.w3schools.com/charsets/ref_html_utf8.asp), ou [W3Schools](https://www.w3schools.com/charsets/ref_emoji.asp). 
    2. Coloque uma barra horizontal de separação `hr` 
    3. Conte a história por palavras suas, mas usando marcadores de estilo (veja slides 17 e 18 da aula) e organizacionais para formatar cada palavra diferentemente 😬!
    4. Coloque uma barra horizontal de separação `hr` 
    5. Conte a história por palavras suas sem formatação. 
4. De seguida, num novo parágrafo apresente o seu website, criando uma lista não numerada onde apresenta em poucas palavras cada uma das páginas do seu website, incluindo um link para essa página numa das palavras.


# Página Localização

Na página `local.html`:
1. Por baixo do menu, insira no elemento `h2` a palavra Localização.
2. Insira um pequeno parágrafo que descreva a localização da ciadade (continente, país), assim como algumas informações geográficas destas.
3.	Insira por baixo um mapa do Google Maps do lugar. Para tal: 
    a. procure o lugar no website www.google.pt/maps
    b. Faça um zoom que considera apropriado
    c. clique em “partilhar” e na opção “incorporar mapa” 
    d. Selecione tamanho pequeno
    e. copie o código HTML resultante, `<iframe src=… >`
    f. insira esse código HTML na sua pagina HTML
    g. acerte a dimensão da janela.


# Página Multimédia

Na página `multimedia.html` crie:
1. Um elemento `h2` com a palavra Multimédia, em vez de Introdução.
2. Pesquise no Youtube por um video sobre a cidade escolhida e insira-o na sua página recorrendo à opção "partilhar" e escolhendo "embeded". Será um elemento ìframe`.


# Página Informações

Na página `info.html`:
1.	Um elemento `h2` com a palavra Informações em vez de Introdução.
2. Crie uma frase a introduzir uma tabela de informações a compilar sobre a cidade.	
3.	Crie uma tabela com dados à sua escolha sobre a cidade escolhida. Deverá ter pelo menos 3 colunas e 4 colunas edeverá usar colspan e rowspan. Uma sugestão é ir à wikipedia e extrair alguns elementos que aparecem numa tabela à direita. A terceira coluna pode consistir num elemento agrupador (por exemplo demografia, geografia, história, etc). Veja o exemplo da tabela nos slides.
4.	Deve depois formatar esta tabela usando os seguintes atributos:
    * pelo menos um atributo rowspan e um coslpan (o valor de cada um sendo maior que 1). 
    * cellspacing,
    * cellpadding, 
    * bgcolor, 
    * align, 
    * border (use border="1"),
    * formatação de colunas com colgroup, explorando os atributos existentes

# Ponha o seu site online

1. Crie uma conta em pythonanywhere.
2. Clique em Web, em "Add a new web app"
3. Next
4. Clique em "Manual configuration"
5. Escolha "Python 3.10"
6. No separador "Files" crie uma pasta intitulada "web"
7. Carregue todos os ficheiros do seu website
8. No separador "Web", clique no botão verde "Reload ...."
9. O seu site está online! Clique no seu dominio
 
# Fim
 
Esperamos que tenhas gostado de aplicar os conhecimentos de HTML fazendo um primeiro website &#127760;!

