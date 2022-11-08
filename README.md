# HTML & CSS

Curso em vídeo - Programação web

Conceitos básicos sobre a web :

## O que é UTF-8?
( Usc tranformation formal 8) é a codificação mais comum da word wide
Web. Cada caractere é representado por um quatro de beats. UTF-8 é compatível com as versões anteriores do ASCII e pode representar qualquer caractere Unicode padrão

---

## Diferença de Mb para MB
MB: megabytes – armazenamento  
Mb: megabite – transmissão

---

## Domínio  

Ele é composto por uma série de componentes como:
- nome único
- pago anualmente
- vários tlds

---

## Hospedagem

- espaço para armazenamento
- pago mensalmente
- espaço, memórias, redes

### Especificando a URL: 
A URL de cada site sempre vai conter os seguintes componentes:  

- domínio: github.com
- tld: .com
- sub.domínio: www.
- caminho: /whoemai

Todos eles formam a URL

- HTML: conteúdo
- CSS: estilo /  design 
- JavaScript: interação com o usuário 

---

## Paragrafo e quebra de linha: 

```<p>``` : serve como marcação e caso queira fazer uma quebra de linha basta usar a tag ```<br>```. Isso porque o que importa são as marcações e não o modo que escreve.

---

## Formatando imagens:
- Diferença entre PNG e JPEG:
- PNG: fundo transparente
- JPEG: imagem compactada sem fundo transparente

Devemos ficar atento ao tamanho dos arquivos para não pesar o nosso site.
Podemos usar imagens tanto da pasta atual quando de sus pastas e links de imagens.

### O que é o favicon?

Todo site tem ícone na sua aba e esse é chamado de favicon, e podemos mudar ele no HTML usando o comando link-favicon.

### Links em HTML:

Podemos colocar links em nossos sites pelo HTML, mas cuidado ao fazer isso pois temos a maneira correta para realizar.

Temos a opção de colocar links em cima de palavras dentro de um ```<p>``` utilizando o comando ```<a>```(ancora),  mas o cuidado aqui é que ao colocar esse tipo de link temos que declarar o seguinte: ```target="_blank" , rel="external"```

A tag ```target``` serve para que o navegador possa abrir o link em uma nova aba e não precisando fechar a atual(seu site) e a tag ```rel``` tem o intuito de dizer ao navegador que este link é externo.

Listas em HTML: 

- listas ```<ol>``` (listas ordenadas)
As listas ordenadas são aquelas que tem uma sequência a seguir como exemplo 1,2,3,4,5. Podemos mudar a numeração da mesma com o comando ```type="1"``` e dizer aonde ela ira iniciar utilizando o ```start="0"```.

- listas ```<ul>``` (listas não ordenadas)
Utilizamos ela para criar listas das quais não temos uma sequência a seguir como, por exemplo, lista de compras.

- Abreviações / Descrições ```<abbr>```
A tag ```<abbr>``` permite colocarmos uma abreviação em nosso texto

---

## Downloads HTML:

Para disponibilizamos um download em nosso site usamos o link ancora ```<a>``` e junto a ele adicionamos o ```type="application/pdf"``` (mas o application pode alterar conforme o arquivo disponibilizado para download para ter acesso à lista completa acesse o link: https://www.iana.org/assignments/media-types/media-types.xhtml)

---

## Imagens Dinâmicas:

Usamos as Imagens Dinâmicas para que o usuário possa ver a mesma img em diferentes tamanhos conforme a tela que ele está utilizando no momento.

Para fazer isso usamos os seguintes comandos: ```<picture>``` e dentro dele usaremos o comando source:media:type sempre fazendo a estrutura das imagens em ordem crescente ou decrescente (p, m ,g) (g, m, p).

Uma dica do Guanabara é usar o ```max-width``` ao invés do ```min-width```.

---

## Psicologia das Cores:

Cada cor tem seu significado, pesquise a importância das cores antes de fazer seu site.

### Fontes: 

Temos os estudos das fontes que mostra que pra cada objetivo do site usamos uma fonte específica.

Tipos de ```format()```
- opentype (otf)
- truetype (ttf)
- embedded-opentype
- truetype-aat (Apple Advenced Typography)
- svg

- Serifa  
    Ela serve para dar ao leito uma melhor leitura das palavras, ideal para textos longos.

- Tamanho  
    Ao decidir o tamanho dos textos do seu site é importante saber que temos dois tipos de tamanho para fontes: 
	
- absolutas  
(cm, mm, in, pt, px, pc)

- relativas  
(em, ex, rem, vh, %)

Conforme as recomendações da w3c usaremos para medidas de fonte o px & em.

- Peso da fonte:  

```font-weight``` – é por esse comando que vamos mudar o peso da nossa fonte
(deixar a letra em negrito)

```font-style``` – é por esse comando que vamos mudar o estilo da fonte (itálico)

```text-decoration``` – é com esse comando que vamos decorar a fonte (Sublinhado)

Vamos simplificar isso usando o shorhand font com o codigo:  
```font: italic, bolder, 3em, “arial”, sans serif;```  
 (font-style → font-weight → font-size → font-family )

---

## Seletores-CSS:

Quando queremos nos referir a um seletor do HTML em específico usamos as tags id e class.

- Id:
Usamos ele para nomear unicamente uma tag, ou seja, não podemos ter mais de um id no mesmo corpo (ter duas tag com o id-iniciante está errado)

- CLASS:
Usamos a class quando queremos ter mais de uma marcação no mesmo corpo, então pra uma única marcação usamos o id e para várias usamos a class.
Podemos tambem colocar mais de uma classe em uma tag como exemplo (class=”avancado destaque”) dentro dessa class temos as modificações do avançado e do destaque, e não precisamos utilizar , para separar as class, para isso usamos o espaço.

Também podemos usar em uma mesma elemento o id e a class, mas o id sobrepõe as configurações da class.

---

## ```# = id```
```
. = class  
: = pseudo-class  
:: = pseudo-element  
> = children
```
---

## O que são caixas em HTML?

As caixas em HTML  servem realmente como um compartimento para guardar algo.
Podemos colocar caixa dentro de outra caixa, isso se chama aninhamento.
Na classificação delas temos dois tipos as box-level e a inline-level

- Box-level:
Ao usar esta caixa nosso HTML ira fazer uma quebra de linha para adicionar a caixa.```<div>```

- Inline-level:
Ao usar esta caixa nosso HTML não faz a quebra de linha. ```<span>```

---

## Tabelas em HTML:

Podemos fazer tabelas nos nossos sites iguais tabelas de excel.  
Mas antes disso precisamos saber como estruturar uma tabela.  
Ela é estruturada da seguinte forma: ```table > caption > thead > tbody > tfoot```  
Fazemos a montagem da tabela como no html aonde temos o cabeça o corpo e o pé.  
Para declarar os dados usamos ```TD``` e para declarar o título usamos o ```TH```.   
E para termos um site de qualidade temos também que fazer o escopo da nossa tabela aonde fazemos com ```scope=" "```
