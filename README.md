**UNIVERSIDADE LUSÓFONA, Programação Web, 22-23**

# Laboratório 1: *O meu primeiro website online* 

## Objetivo
* Criar um website **sobre uma cidade ou lugar à sua escolha**.
* Aplicar os conceitos elementares de HTML.
* Colocar o website online

## Prazo de Entrega
* Este laboratório deverá ser concluido até dia 19.2, sendo posteriormente avaliado. 

## Pré-requisitos
* Instale o VS Code para editar o código HTML de forma fácil.
* Instale no VS Code a extensão live server. Permitir-lhe-á visualizar a página renderizada, à medida que for editando. Basta clicar, no canto inferior direito, em `Go live`.
* Utilize `Shift+Alt+F` para indentar código

# 1. HTML `<>`

O HTML é uma linguagem de marcação para construir páginas Web. Os ficheiros HTML possuem marcadores (*tags*), palavras entre parênteses angulares (`<` e `>`) que são comandos de formação da linguagem. 

Por exemplo, no elemento `<title>Primeira página</title>`:
* `<title>` é o marcador de abertura
* `</title>` é o marcador de fecho
* `Primeira página` será o conteúdo afetado pelo marcador <title>, que neste caso especificará o título da barra de navegação.

 Reveja se necessário os slides da [aula prática](https://github.com/ULHT-PW/pw23-lab1/files/10727143/pw-lab1.pdf)

<details>
 
 <summary>Marcadores usados neste laboratório</summary>

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

</details>


# 2. A minha primeira página HTML 😀 

Fará neste laboratório um website sobre uma cidade do mundo à sua escolha que goste. Deverá congregar várias informações sobre esta conforme indicado ao longo do laboratório. 

1. crie uma pasta `lab1` e abra-a com o VSCode.  

2. crie o ficheiro `index.html`, inserindo as seguintes partes elementares de qualquer ficheiro HTML:

![image](https://user-images.githubusercontent.com/42048382/218617086-1675ad42-c35a-4ee3-aabb-0be3e40218bb.png)

3. Dentro do elemento `<head>` insira os seguintes elementos:
    1. `<title>`, com o nome da cidade escolhida, que especificaráo título da barra do navegador. 
    2. `<meta charset="utf-8">`, metadado (meta) que especifica que a página utiliza UTF-8 como codificação de carateres, em vez de ASCII. Isso permite inserir emojis e carateres não ASCII tipo ç, ã, õ. 
    3. nome do autor do site, descrição do conteudo do site, e palavras chave: 
        * `<meta name="author" content="Ana Maria">`
        * `<meta name="description" content="Website sobre Lisboa">`
        * `<meta name="keywords" content="palavras chave">`

4. No corpo principal, `<body>`: 
    1.	insira um elemento `<h1>` com o nome da cidade.
    2.	Procure no Google uma imagem que goste da cidade. 
    3. Edite-a com o Paint. Redimensione-a proporcionalmente para que tenha 300px de largura. 
    3. Guarde a imagem numa nova pasta `images`. 
    4. Insira a imagem usando a etiqueta `<img>`. Especifique no atributo `src` o caminho até ao ficheiro.
    5.	Insira, depois da imagem, uma quebra de linha, elemento `<br>`, pois o elemento `<img>` não introduz uma quebra de linha.
    6. Insira por baixo um titulo `<h2>` com a palavra Introdução 
    7. Escreva uma frase sobre a cidade.

 ![image](https://user-images.githubusercontent.com/42048382/218616647-c7377b2e-e9d3-48de-8310-8eb047647970.png)
 
A sua página está pronta!   
1. visualize a sua pagina, clicando diretamente no ficheiro HTML na pasta. O seu browser abrirá e renderizará a página.
2. visualize a sua pagina, clicando no canto inferionr direito em "Go live". Deixe sempre aberto. Todas as alterações que for  fazendo serão automaticamente refrescadas.
    
Está ligeiramente diferente da imagem a cima, pois falta inserir os hiperlinks.

# 3. Mais páginas para o meu website! 🥳

Irá agora criar várias páginas interligadas, como no [slides 15](https://github.com/ULHT-PW/pw23-lab1/files/10727143/pw-lab1.pdf#page=15) da aula prática.

1. Crie o menu depois da imagem e etiqueta `<br>`. Num `<p>` coloque 4 hiperlinks `<a>` para as páginas do seu site: Introdução, Localização, Multimédia, Informações. 

![image](https://user-images.githubusercontent.com/42048382/218616401-14dcee38-e524-42bd-ad50-773df147a1be.png)


2.	Crie 4 copias do ficheiro index.html que criou. 
3.	Altere os nomes dos ficheiros para ter os seguintes: index.html, local.html, multimedia.html, info.html (atenção que os nomes dos ficheiros HTML  deverão estar em minúsculas, sem espaços, acentos ou carateres especiais)
4.	Em cada ficheiro, no menu, ponha a negrito a palavra a que corresponde a página. Para pôr a negrito colocque a etiqueta `b`em volta do hiperlink devido.
5. Adeque o título `<h3>Introdução</h3>` ao nome da página.
6. Abra o ficheiro index, e verifique que os hiperlinks funcionam. 
Tem agora criado o seu website! Agora irá preencher cada página com conteúdos.
    
# 4. Site online em 10 passos! ☁

1. Crie uma conta em [www.pythonanywhere.com](https://www.pythonanywhere.com/). O username que escolher será o nome do seu dominio (username.pythonanywhere.com). 
![image](https://user-images.githubusercontent.com/42048382/218605220-87f17a31-df30-45c9-941a-812145bcbfd7.png)
2. No menu superior, clique em "Web" e depois em  "Add a new web app"
3. Clique em "Manual configuration"
4. Escolha "Python 3.10"
5. No menu superior, clique em "Files"
6. crie uma pasta intitulada "web"
7. Carregue nessa pasta todos os ficheiros do seu website
8. No menu superior, clique em "Web"
9. No separador Static, especifique em URL  `/`, e em Directory o caminho até à sua pasta web
10. Clique no botão verde "Reload ...."
11. Clique no seu dominio. O seu site está online 🥳
    
Continue a editar no VS Code o seu website. No final, carregará os ficheiros finalizados. 
    
# 5. Página Introdução 🏕

Na pagina `index.html` insira, por debaixo da frase que escreveu sobre a cidade crie:

1. De seguida, num novo parágrafo `<p>` apresente o seu website, criando uma lista não numerada com a etiqueta `<ol>` e várias linhas `<li>`. Em cada linha apresente cada página do seu site em poucas palavras, incluindo numa palavra chave um link para essa página, com o elemento `<a>`.

2. Crie uma [wordcloud](https://www.wordclouds.com/) com base em palavras que associa à cidade. 
    1. Clique em wordlist e Edit, prima no botão para apagar as palavras existentes.
    2. Adicione palavras que estejam associadas à cidade. 
    3. Ponha peso 10 no nome da cidade para que esta fique com maior destaque. 
    4. Pode escolher uma forma (shape), fonte (font), cores (use um fundo branco). 
    5. Descarregue a imagem, e formate-a com o Paint por forma a que tenha largura de 300px como a fotografia da cidade. 
    6. Guarde a imagem na pasta `/images`
    6. Insira-a como uma `<img>` por debaixo da lista.

# 6. Página Localização 🗺

Na página `local.html`:
1. Insira um pequeno parágrafo que descreva a localização da ciadade (continente, país), assim como algumas informações geográficas destas.
2.	Insira por baixo um mapa do Google Maps do lugar. Para tal: 
    a. procure a cidade no website www.google.pt/maps
    b. Faça um zoom que considera apropriado
    c. clique em “partilhar” e na opção “incorporar mapa” 
    d. Selecione tamanho pequeno
    e. copie o código HTML resultante, `<iframe src=… >`
    f. insira esse código HTML na sua pagina HTML
    g. acerte a dimensão da janela.


# 7. Página Multimédia 🎬

Na página `multimedia.html` crie:
1. Pesquise no Youtube por um video sobre a cidade escolhida e insira-o na sua página recorrendo à opção "partilhar" e escolhendo "embeded". Será um elemento ìframe`.


# 8. Página Informações ℹ

Na página `info.html`:
1. Crie uma frase a introduzir uma tabela de informações a compilar sobre a cidade.	
2. Crie uma `<table>` com dados à sua escolha sobre a cidade escolhida (consulte, e.g., Wikipedia).
    
# 9. Site atualizado online!

1. Na aplicação [pythonanywhere](https://www.pythonanywhere.com/), clique em "Files"
7. Carregue pasta todos os ficheiros do seu website, pois muitos foram modificados
8. No menu superior, clique em "Web"
9. Clique no botão verde "Reload ...."
10. Clique no seu dominio. O seu site está online 🥳
    
 
# 10. Fim 🎉

Submeta o domínio da sua aplicação no Moodle até à sua próxima aula prática

Esperamos que tenha gostado de aplicar os conhecimentos de HTML fazendo um primeiro website &#127760;!

