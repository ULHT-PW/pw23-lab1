**UNIVERSIDADE LUSÓFONA**

# Programação Web - Laboratório 1: <br>*O meu primeiro website* 

## Objetivo
* Neste laboratório criará um website sobre uma cidade à sua escolha, onde irá aplicar os conceitos elementares de HTML.
* Este laboratório deverá ser concluido antes da sua aula prática da semana de 20.2, onde será avaliado. 

## Recomendações
* Leia o enunciado todo com atenção antes de o começar a resolver para entender o que fará.
* Execute com atenção cada passo, certificando-se que implementa todos os detalhes.  
* Se tiver alguma dúvida, recorra aos slides que contêm os conhecimentos que precisa para realizar o laboratório.

## Pré-requisitos
* Deverá ter o VS Code instalado para editar o código HTML de forma fácil.
* Instale no VS Code a extensão live server. Permitir-lhe-á visualizar a página, à medida que for editando. Basta clicar, no canto inferior direito, em `Go live`.
* Para que o seu código fique bem indentado, utilize o comando `Shift+Alt+F`

# HTML

O HTML é uma linguagem de marcação para construir páginas Web. OS ficheiros HTML possuem marcadores (*tags*), palavras entre parênteses angulares (`<` e `>`) que são comandos de formação da linguagem. 

Reveja se necessário os slides apresentados na [aula prática](https://github.com/ULHT-PW/pw23-lab1/files/10727143/pw-lab1.pdf)

Por exemplo, no elemento `<title>Primeira página</title>`:
* `<title>` é o marcador de abertura
* `</title>` é o marcador de fecho
* `Primeira página` será o conteúdo afetado pelo marcador <title>, que neste caso especificará o título da barra de navegação.

Neste laboratório utilizará vários marcadores:
* `<h1>` = marcador que define um titulo - heading1 (`<h2>` um subtítulo, `<h3>` um subsubtítulo, ...)
* `<p>` = marcador que define um parágrafo
* `<ul>` = marcador que define uma lista não numerada (`<ol>` para lista numerada)
* `<li>` = marcador que define uma linha
* `<img>` = marcador que define uma imagem
* `<a>` = marcador de âncora para hiperlink, especificado como valor do atributo `href` 
* `<table>` = marcador que define uma tabela
* `<tr>` = marcador que define uma linha (*table row, tr*) duma tabela
* `<td>` = marcador que define uma célula (*table data, td*) duma tabela

Dentro de um marcador podem ser especificados pares de `atributo="valor"`. Os atributos modificam os resultados padrões dos elementos e os valores caracterizam essa mudança. Utilizará os seguintes atributos:
* `src` = atributo que define o nome do ficheiro com a imagem
* `href`= atributo que define o URL da hiperligação
    
Nas próximas aulas falaremos mais em detalhe destes aspectos.


# 1. Página Web 

Fará neste laboratório um website sobre uma cidade do mundo à sua escolha que goste. Deverá congregar várias informações sobre esta conforme indicado ao longo do laboratório. 

1. crie uma pasta `lab1` e abra-a com o VSCode.  

2. crie o ficheiro `index.html`, inserindo as seguintes partes elementares de qualquer ficheiro HTML:

```html
<!DOCTYPE html>
<html lang="pt">
    <head>
    </head>
    <body>
    </body>
</html>
```

1. Dentro do elemento <head> insira os seguintes elementos:
    1. `<title>`, com o nome da cidade escolhida, que especificaráo título da barra do navegador. 
    2. `<meta charset="utf-8">`, metadado (meta) que especifica que a página utiliza UTF-8 como codificação de carateres, em vez de ASCII. Isso permite inserir emojis e carateres não ASCII tipo ç, ã, õ. 
    3. nome do autor do site, descrição do conteudo do site, e palavras chave: 
        * `<meta name="author" content="Ana Maria">`
        * `<meta name="description" content="Website sobre Lisboa">`
        * `<meta name="keywords" content="palavras chave">`

# 2. A minha primeira página

Crie agora a sua primeira página. Siga o template em baixo: terá no topo o nome da sua cidade, uma imagem à sua escolha e o menu, ficando da seguinte forma:

![cabecalho](https://user-images.githubusercontent.com/42048382/218595546-59a5863a-0f14-4002-8176-80d2ae3b2aa2.png)

Para, tal, siga os seguintes passos (reveja os slides da aula prática): 
1.	No body, insira um elemento `h1` com o nome da cidade.
2.	Na linha seguinte insira uma imagem da cidade a seu gosto. Redimensione a imagem para que tenha 300px de largura. No Paint existe uma opção resize que lhe permite escolher o número de pixels que pretende que tenha de largura. Respeite a proporção da imagem, sem a deformar! 
3. Guarde a imagem numa nova pasta `images`. 
4. Insira a imagem usando a etiqueta `img`. Especifique no atributo `src` o caminho até ao ficheiro, ficando `<img src="images/cidade.png">`.
    
5.	Insira, depois da imagem, uma quebra de linha, elemento `<br>`, pois o elemento `<img>` não introduz uma quebra de linha.

4. Insira um titulo `h2` com a palavra Introdução 
5. Finalmente, escreva uma frase sobre a cidade.

    
A sua página está pronta!   
1. visualize a sua pagina, clicando diretamente no ficheiro HTML na pasta. O seu browser abrirá e renderizará a página.
2. visualize a sua pagina, clicando no canto inferionr direito em "Go live". Deixe sempre aberto. Todas as alterações que for  fazendo serão automaticamente refrescadas.
Para está ligeiramente diferente da imagem a cima, pois falta inserir os hiperlinks.

# 3. Mais páginas para o meu website!

Irá agora criar várias páginas interligadas, como no slide da aula prática. Reveja os [slides 15 e 16](https://github.com/ULHT-PW/pw23-lab1/files/10727143/pw-lab1.pdf) PAra tal:
1. Crie o menu. Para tal:
    1. Depois da imagem e etiqueta `<br>`, crie o menu.Crie um parágrafo `<p>` com cinco elementos de hiperlink `<a>`, tendo como conteúdo o nome das páginas do seu site: Introdução, Localização, Multimédia, Informações, Home, estando os elementos separados pelo carater `|`. 
    2. Use como valor para o atributo `href` as seguintes páginas:
        1. `index.html` para Introdução 
        2. `local.html` para Localização
        3. `multimedia.html` para Multimédia
        4. `info.html` para Informações

2.	Crie 4 copias do ficheiro index.html que criou. 
3.	Altere os nomes dos ficheiros para ter os seguintes: index.html, local.html, multimedia.html, info.html (atenção que os nomes dos ficheiros HTML  deverão estar em minúsculas, sem espaços, acentos ou carateres especiais)
4.	Em cada ficheiro, no menu, ponha a negrito a palavra a que corresponde a página. Para pôr a negrito colocque a etiqueta `b`em volta do hiperlink devido.
5. Adeque o título `<h3>Introdução</h3>` ao nome da página.
6. Abra o ficheiro index, e verifique que os hiperlinks funcionam. 
Tem agora criado o seu website! Agora irá preencher cada página com conteúdos.
    
# 4. Site online em 10 passos!

1. Crie uma conta em [www.pythonanywhere.com](https://www.pythonanywhere.com/). O username que escolher será o nome do seu dominio (username.pythonanywhere.com). 
![image](https://user-images.githubusercontent.com/42048382/218605220-87f17a31-df30-45c9-941a-812145bcbfd7.png)
2. No menu superior, clique em "Web" e depois em  "Add a new web app"
3. Clique em "Manual configuration"
4. Escolha "Python 3.10"
5. No menu superior, clique em "Files"
6. crie uma pasta intitulada "web"
7. Carregue nessa pasta todos os ficheiros do seu website
8. No menu superior, clique em "Web"
9. Clique no botão verde "Reload ...."
10. Clique no seu dominio. O seu site está online 🥳
    
Continue a editar no VS Code o seu website. No final, carregará os ficheiros finalizados. 
    
# 4. Página Introdução

Na pagina `index.html` insira, por debaixo da frase que escreveu sobre a cidade crie:
3. Pequena história divertida:  
    1. Conte uma pequena história divertida apenas com emojis 😉, sobre a :cityscape: que escolheu. Explore emojis, premindo nas teclas `🙂Windows + .`, ou pesquise na Internet em [emojipedia](https://emojipedia.org/), [carateres especiais UTF-8](https://www.w3schools.com/charsets/ref_html_utf8.asp), ou [W3Schools](https://www.w3schools.com/charsets/ref_emoji.asp). 
    2. Coloque uma barra horizontal de separação `hr` 
    3. Conte a história por palavras suas sem formatação. 
4. De seguida, num novo parágrafo apresente o seu website, criando uma lista não numerada com a etiqueta `<ol>` e várias linhas `<li>`. Em cada linha apresente cada página do seu site em poucas palavras, incluindo numa palavra chave um link para essa página, com o elemento `<a>`.
5. Crie uma [wordcloud](https://www.wordclouds.com/) com base em palavras que associa à cidade. 
    1. Clique em wordlist e Edit, prima no botão para apagar as palavras existentes.
    2. Adicione palavras que estejam associadas à cidade. 
    3. Ponha peso 10 no nome da cidade para que esta fique com maior destaque. 
    4. Pode escolher uma forma (shape), fonte (font), cores (use um fundo branco). 
    5. Descarregue a imagem, e formate-a com o Paint por forma a que tenha largura de 300px como a fotografia da cidade. 
    6. Guarde a imagem na pasta `/images`
    6. Insira-a como uma `<img>` por debaixo da lista.

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

    
# Site atualizado online!

1. Na aplicação [pythonanywhere](https://www.pythonanywhere.com/), clique em "Files"
7. Carregue pasta todos os ficheiros do seu website, pois muitos foram modificados
8. No menu superior, clique em "Web"
9. Clique no botão verde "Reload ...."
10. Clique no seu dominio. O seu site está online 🥳
    
 
# Fim
 
Esperamos que tenha gostado de aplicar os conhecimentos de HTML fazendo um primeiro website &#127760;!

