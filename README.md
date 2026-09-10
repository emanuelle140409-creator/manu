https://emanuelle140409-creator.github.io/manu/


## 1. construção de textos e parágrafos com HTML

### A. criação de parágrafos ou frases 

#### Exemplo:
```html
<p id = "p1" onclick = "mudar_cor()">Aqui vai qualquer texto ou frase que queira</p>
```
## B.Adicionando CSS aos parágrafos

#### Exemplo adicionando cores:
```css
#p1{

    color: blue;

}
```
### C.Adicionando JavaScript aos parágrafos

#### Exemplo mudando cores:
```js
function mudar_cor(){

    document.getElementById("p1").style.color = "brown";

}
```
### Observe que o mesmo p1 está sendo repetido no HTML, CSS e JavaScript!!!

<br>

## 2. Construção de títulos e subtítulos

### A. Toda página possui um único tema. Para isso, use h1.

<h1 id ="mudar_h1()">Tema da minha página</h1>

<br>

### B.Adicionando um tipo de capitalização:

#### Exemplo adicionando um tipo de capitalização

#h1{

    text-transform: lowercase;
}

<br>

### C. ADICIONADO JAVASCRIPT AO TEMA 

### EXEMPLO MUDANDO A CAPITALIZAÇAO PADRÃO DO CSS:

fuction mudar_h1(){
    
    document.getElementById("h1").style.textTransform = "uppercase";
}

### D.Toda página pode tersubtitulos para cada pedaço de conteúdo,assim como um mercado possui um nome para cada corredor.. Para isso,use h2.
```
<h2 id = "h2" onclick ="mudar_h2()">Subtítulo da seção frutas</h2>

<h2 id = "h2" onmouseenter ="mudar_h2()">Subtítulo da seção frios</h2>

<br>

### E. Adicionando CSS aos subtítulos

#### Exemplo adicionando cor de fundo e alterando alinhamento:
```css
#h2{

    background-color: cyan;
}
```
#h_2{

    text-align: rigth;
}

<br>

### F.Adicionando JavaScrit ao subtítulos

#### Exemolo mudando a cor de fundo e o alinhamento padrão do CSS.
```js
fuction mudar_h2(){ 

    document.getElementById("h2").style.backgroundColor = "yellow";
}

fuction mudar_h_2(){
    
    document.getElementById("h2").style.backgroundColor = "left";;
}  
```
<br>

### 3. Construção listas ordenadas e desordenadas

<br>

### A) Listas Ordenadas : agrupar itens que possuem uma relação de ordem crescente ou decresecente entre si.

### Exemplo 
```html
<h1>SEleções nacionais mais vencedoras da copa do mundo FIFA :</H1>
<ol id ="ol1" onclick = "mudar_ol1()">
<li>Brasl - 5</li>
<li>Alemanha - 5</li>
<li> Itália - 5</li>
<li>Argentina - 5</li>
<li>Uruguai - 5</li>
<li>França - 5</li>
<li>Espanha - 5</li>
<li>Inglaterra - 5</li>
</ol>
```
<br>

### B) Customizando com o CSS


#### EXEMPLO ALTERANDO O TIPO DE ORDENAMENTO E SUA COR:
```
#ol1{
    list-style-type: lower alpha;
}

#ol1 > li::marker{
    color : red;
}
```
<br>

### C)Adicionando interação com o JS.

#### Exemplo modificando o tipo de ordenamento:
```
function mudar_ol1(){
    document.getElementById("ol1").style.listStileType = "decimal";
```
}
<br>

### D) Listas não ordenadas : agrupar itens que não possuem uma relação de ordem crescente ou decresecente entre si.

### Exemplo
```
<h1>Os assuntos mais comuns em estatística</h1>

<ul id ="ul1" onclick = mudar_ul1()">

<li>Média</li>
<li>Moda</li>
<li>Mediana</li>
<li>Variancia</li>
<li>Amostragem</li>
<li>Desvio padrão</li>
<li>Intervalo de confiança</li>
</ul>
```
<br>

 ### E) Customizando com o CSS

 #### Exemplo alterando o símbolo de destaque aso lado do nome e sua cor:
```
 #ul1{
    list-style-type: square;
 }

 #ul1> li:marker{
    color:coral;
 }
```
 <br>

 ### F) Adicionando interação com o JS.

 #### Exemplo modificando o símbolo de destaque
 ```
 function mudar_ul1(){
        document.getElementById("ul1").style.listStileType = "circle";
```
 }
<br>

### 4. imagens
<br>

### A) Imagens por padrão em um site:
#### Exemplo:
<Figure>
<img id = "gif0" onmouseenter = "mudar_gif0()" src=" ./imagens/html/-css-js.gif" alt= "GIF com diferena entre HTML, CSS e Javascript" width="480" height= "480">
</figure>
<br>

### B)Custumizando com o CSS
#### Exemplo adicionando arredondamento da borda, opacidade,borrão brilho e sombreado de uma imagem:
<br>

# gif0{
    border-radius: 30px;
    opacity: 0.8;
    filter: blur(2px) brightness (150%) drop-shadow(10px 10px 1px red);
}
<br>

### C) Adicionando interação com o JS.

#### Exemplo modificando a imagem:

fuction mudar_gif0(){
    
document.getElementById("gif0").style.borderRadius = "15px";
document.getElementById("gif0").style.opactiy = "0,7";
document.getElementById("gif0").style.filter= "blur(3px)";
document.getElementById("gif0").style.filter= "brightness(70%)";
document.getElementById("gif0").style.filter= "drop-shadow(6px 7px 2px coral)";
}

<br>

### 5.videos
<br>

#### ) Vídeos por padrão em um site

#### Exemplo:
<vídeo id= "vídeo_0" width = "640" height = "360" controls>
<source src = "./videos/movie1.mp4" type= "video/mp4>
</video>
<br>

### B) Videos vindo do youtube com iframe

#### Exemplo:

<iframe width="640" height="360" src="https://www.youtube.com/embed/LXb3EKWsInQ"TITLE="COSTA RICA IN 4K 60FPS HDR (ULTRA HD)" allowfyllscreen></iframe>
<br>

### C) Customizando com o CSS

#### Exempllo adicionando arredondamento da borda e sombreando no vídeo:
<br>
#vídeo_0{
    border-radius: 10px;
    filter: drop-shadow (2px 2x 5px gray);
    ]
     <br>
    
    ## 6. HIperlinks

    <br>

    ### A) HIperlinks para outros sites

    #### Exemplos abrindo o link na mesma aba do navegador:
    <nav>
    <a id="link_0"href = "https://www.youtube.com" target ="_blank" >Google</a>
</nav>

#### Exemplo abrind o link n\ mesma aba do navegador:
<nav>
    <a id="link_0"href = "https://www.youtube.com">youtube</a>
    </nav>
<br>
/* a aparencia padrão do link */
#link_0:link {
    colror: magenta;
    transition: font-size 2s;
}
/*segundos após o link ser clicado a aparencia do link é alterada*/
#link_0:visited{
    color: none;
}
/*alterar a aparencia quando o mouse passa por cima (hover) do link */
#link_0:hover{
    color: hotpink;
    font-size: 2em;
    transition: font-size 2s;
}
/*altera a coor no exato momento que o link é clicado com o mouse*/
#link_0:actve {
    color:none;
}

