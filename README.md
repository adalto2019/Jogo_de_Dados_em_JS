## Jogo de Dados em JS
Aqui foi desenvolvido um jogo de dados multiplayer, para dois jogadores, como requisito de avaliação dissertativa do curso de FULLSTACK. Instruções: os jogadores definirão antecipadamente quantos dados serão rolados por partida. Ex. "melhor de três": o primeiro jogador inicia o lançamento, em seguida o segundo jogador inicia o seu laçamento. E continua assim por diante até chegar no limite de laçamentos previamente definidos da partido (Nesse exemplo três lançamentos para cada jogador). 
No final, conta-se o histórico de ponto armazenado de cada um, vencendo quem tiver alcançado a maior pontuação.

## Layout do Projeto
<img src = "ImgPrintJogo.png">

## Tecnologias Utilizadas
Front End: HTML5, CSS e JavaScript

## Inspecionando o Código
~~~JavaScript
<script>
        var res1 = document.getElementById("res1")
        var res2 = document.getElementById("res2")
        var imgs1 = document.getElementById("imgs1")
        var imgs2 = document.getElementById("imgs2") 
        var arrayPC = []
        var arrayJG = []
        function lancarPC(){ 
            c = Math.floor(Math.random() * 6 ) + 1
            //'6' define qtd de numeros a ser sorteados (o index começa em zero). '1' define de que numero começa.
            Nsorteado = Number(c)
            arrayPC.push(Nsorteado)
            res1.innerHTML = "Histórico dos números sorteados: " + arrayPC //valor que substitui a variável resultado
            if (c == 1){
                imgs1.innerHTML = "<img src=img1.jpeg>"
            }
            if (c == 2){
                imgs1.innerHTML = "<img src=img2.jpeg>"
            }
            if (c == 3){
                imgs1.innerHTML = "<img src=img3.jpeg>"
            }
            if (c == 4){
                imgs1.innerHTML = "<img src=img4.jpeg>"
            }
            if (c == 5){
                imgs1.innerHTML = "<img src=img5.jpeg>"
            }
            if (c == 6){
                imgs1.innerHTML = "<img src=img6.jpeg>"
            }
        }
        function lancarJG(){ 
            c = Math.floor(Math.random() * 6 ) + 1
            //'6' define qtd de numeros a ser sorteados (o index começa em zero). '1' define de que numero começa.
            Nsorteado = Number(c)
            arrayJG.push(Nsorteado)
            res2.innerHTML = "Histórico dos números sorteados: " + arrayJG //valor que substitui o resultado     
            if (c == 1){
                imgs2.innerHTML = "<img src=img1.jpeg>"
            }
            if (c == 2){
                imgs2.innerHTML = "<img src=img2.jpeg>"
            }
            if (c == 3){
                imgs2.innerHTML = "<img src=img3.jpeg>"
            }
            if (c == 4){
                imgs2.innerHTML = "<img src=img4.jpeg>"
            }
            if (c == 5){
                imgs2.innerHTML = "<img src=img5.jpeg>"
            }
            if (c == 6){
                imgs2.innerHTML = "<img src=img6.jpeg>"
            }
        }
    </script>
~~~

~~~Css
<style>
        body{text-align: center;
        background-image: url(imgDados.jfif);
            }   
        h1{background-color: black;
            color: wheat;
            font-size: 30px;
            }
        form{background: white;
            width: 400px;
            margin-left: 450px;
            }
         #Placar{background-color: white;
            margin-left: 1000px;
            }       
</style>
~~~

## Autor

Adalto Carvalho Ribeiro Simão Junior - Nov.22

