        <template>
    <div id="container-principal">

        <main>

            <article>
             
                <div class="introducao-ao-conteudo">
                    <section class="banner-video">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/Ss3-T8asuPg?si=qkhkCjIQZxy-l2XI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
                    </section>
                    <section class="sobre-video">
                        <h1>Tudo começa em você</h1>    
                        <p>Com o eBook Tudo Começa em Você, aprenda os 7 passos essenciais para planejar, lançar e vender seus produtos na internet. Encontre um guia prático e direto ao ponto, com linguagem simples e exemplos práticos, ideal para iniciantes que querem abrir sua própria loja online e transformar uma ideia em um negócio lucrativo.</p>
                    </section>
                </div>

                <div class="promocao-desconto">
                    <section class="titulo-do-anuncio">
                        <h1>Comprando agora, você ganha um desconto especial!</h1>
                        <p>Não perca tempo e aproveite essa oferta por tempo limitado que preparamos para você!</p>
                        <a href="https://pay.hotmart.com/F98346505C?off=yep0umya&_hi=eyJjaWQiOiIxNzQxOTE1MTYwMjU1ODk4MjY3ODI5NzI5MDgxOTAwIiwiYmlkIjoiMTc0MTkxNTE2MDI1NTg5ODI2NzgyOTcyOTA4MTkwMCIsInNpZCI6ImIxYjUzNDMyMGM2NTQ1NTA4MDQ0N2I0ZjQzYTJjYThjIn0=.1742927436002" target="_blank" rel="noopener noreferrer">COMPRE AGORA</a>  
                    </section>
                    <section id="contador-promocional"> <!-- Contador promocional -->
                        <span>
                            <p id="horas">00</p>
                            <small>Horas</small>
                        </span>
                        <span>
                            <p id="minutos">30</p>
                            <small>Minutos</small>
                        </span>
                        <span>
                            <p id="segundos">00</p>
                            <small>Segundos</small>
                        </span>
                    </section>
                </div>

                <div class="feedbacks-leitores">
                    <section class="mensagem-representativa">
                        <h3>FEEDBACKS CLIENTES</h3>
                        <small>Conheça outras pessoas, exatamente igual a você, que conseguiram alcançar os resultados!</small>
                    </section>
                    <section class="opnioes-leitores">
                        <span>
                            <img src="../../assets/icon-user.png" alt="icone de usuario">
                            <p>“O eBook Tudo Começa em Você foi um divisor de águas na minha vida. Aprendi a planejar, lançar e vender meus produtos na internet de forma simples e prática. Recomendo a todos que querem abrir sua própria loja online!”</p>
                            <small>João Silva</small>
                        </span>
                        <span>
                            <img src="../../assets/icon-user.png" alt="icone de usuario">
                            <p>“Com o eBook Tudo Começa em Você, aprendi a transformar uma ideia em um negócio lucrativo. O guia prático e direto ao ponto me ajudou a abrir minha loja online e alcançar resultados incríveis!”</p>
                            <small>Maria Santos</small>
                        </span>
                        <span>
                            <img src="../../assets/icon-user.png" alt="icone de usuario">
                            <p>“O eBook Tudo Começa em Você é um verdadeiro manual para quem quer abrir sua própria loja online. Com linguagem simples e exemplos práticos, aprendi os 7 passos essenciais para planejar, lançar e vender meus produtos na internet!”</p>
                            <small>Carlos Oliveira</small>
                        </span>
                    </section>
                </div>

                <div class="ebook">
                    <section class="descricao-livro">
                        <small>Portanto, conheça já o nosso livro!</small>
                        <h3>Tudo Começa em Você: 7 Passos para Criar Sua Loja Online e Começar a Vender</h3>
                        <p>Aprenda desde a escolha do nicho até estratégias de marketing para atrair clientes e aumentar suas vendas. Transforme uma ideia em um negócio lucrativo.</p>
                    </section>
                    <section class="fotografia-livro">
                        <img src="./../../assets/liberarte-ebook.png" alt="">
                    </section>
                </div>

                <div id="sobre" class="sobre-autor">
                    <section class="descricao-autor">
                        <h3>José Liberato</h3>
                        <small>Escritor, Compositor e Radialista</small>
                        <p>Olá! Eu sou José Liberato, sempre busco atender às expectativas dos meus clientes. Levantar e fazer algo é o ingrediente mais importante. É simples assim. Muitas pessoas têm ideias, mas poucas decidem agir hoje, e não amanhã, não na próxima semana, mas hoje. O verdadeiro empreendedor age em vez de apenas sonhar. Apenas aqueles que ousam enfrentar grandes fracassos alcançam grandes sucessos. Um empreendedor enxerga oportunidades onde os outros só veem problemas. Vamos em frente!</p>
                    </section>
                    <section class="fotografia-do-autor">
                        <img src="./../../assets/joselib-autor.jpg" alt="autor fotografia">
                    </section>
                </div>

            </article>
        </main>

        <footer>
            <section class="links-rodape">
                <small>All Right Reserved 2025 - Developed by Rodrigo Liberato</small>
                <img src="./../../assets/logo-liberarte.png" alt="">
            </section>
            
        </footer>
    </div>
</template>
        
<script>
export default {
  name: 'paginaInicial',
  methods: {
    irParaTermos() {
        this.$router.push('termosDeUso'); //Tentar corrigir depois
    }
  }
}


// Função para o contador promocional

// Aguarda o carregamento completo do DOM antes de executar o código
document.addEventListener('DOMContentLoaded', () => {
    // Seleciona os elementos HTML que exibem os minutos e segundos
    let minutes = document.getElementById('minutos');
    let seconds = document.getElementById('segundos');

    // Define o tempo restante em segundos (30 minutos * 60 segundos)
    let tempoRest = 30 * 60;

    // Função para atualizar o contador
    const updateCont = () => {
        // Calcula os minutos restantes dividindo o tempo total por 60
        const min = Math.floor(tempoRest / 60); 
        // Calcula os segundos restantes pegando o resto da divisão por 60
        const sec = tempoRest % 60;

        // Atualiza os elementos HTML com os minutos e segundos formatados
        minutes.innerHTML = `${min.toString().padStart(2, '0')}`;
        seconds.innerHTML = `${sec.toString().padStart(2, '0')}`;

        // Decrementa o tempo restante a cada chamada
        tempoRest--;

        // Para o intervalo quando o tempo chega a zero
        if (tempoRest < 0) {
            clearInterval(interval);
        }
    };

    // Atualiza o contador imediatamente ao carregar a página
    updateCont();
    // Chama a função de atualização a cada 1 segundo (1000 ms)
    const interval = setInterval(updateCont, 1000);


});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    /* Reset CSS */
    * {
        box-sizing: border-box;
        padding: 0;
        margin: 0;  
    }

    html {
        margin: 0 ;
        padding: 0;
        overflow-x: hidden;
        width: 100%;
        min-height: 100vh;
        border: none;
    }
    
    #container-principal { /*Estilização do container principal */
        width: 100vw;
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        background-image:  linear-gradient(to bottom, #0D0D0D 5%, #800020  100%);
        align-items: center;
        color: #F2F2F2;
        margin: 0;
        padding: 0;
    } 

    
    main { /*Estilização do corpo principal */
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 100vw; /*100% do viewport de diferente dispositivos*/
        min-height: 100vh;
        margin: 0 auto;
        padding: 0;
    }

    article  { /*Estilização do artigo principal e a introducao ao conteudo como a demais variacoes*/
        display: flex;
        flex-direction: column; 
        max-width: 1200px;
        width: 100vw; /*100% do viewport em todos os dispotivios */
        min-height: 100vh;
        padding: 0;
        margin: 0 auto;
    }
    
    .introducao-ao-conteudo { /*Estilização do container de introdução ao conteudo */
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        max-width: 1200px;
        width: 100vw;
        height: auto;
        margin: 0 auto;
    }

    .banner-video { /*Estilização do vídeo principal */
        display: flex;
        justify-content: center;
        align-items: center;
        width: 660px;
        height: 515px; 
        margin: 0 auto;
        
    }

    .banner-video iframe { /*Estilização do iframe do video */
        border-radius: 20px;
        box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
    }
    
    .sobre-video { /*Estilização do container sobre o video     */
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 452px;
        height: 515px;
    }

    .sobre-video h1{ /*Estilização do titulo no container sobre o video */
        font-size: 34px;
        font-weight: 900;
        margin: 0;
        padding: 0;
    }

    
    .promocao-desconto { /*Estilização do container do desconto ao cliente */
        display: flex;
        flex-direction: row;
        max-width: 1200px;
        width: 100vw;
        height: auto;
        margin: 0 auto;
        background-color: #800020;
        padding-top: 50px;
        padding-bottom: 50px;
        border-radius: 4px 125px 4px 125px;
        
     
    }

    .titulo-do-anuncio { /*Estilização do container do anuncio */
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        justify-content: center;
        width: 350px;
        height: auto;
        margin: 0 auto;
        padding-top: 70px;
    }

    .titulo-do-anuncio h1 { /*Estilização do titulo do livro */
        font-size: 20pt;
        font-weight: 900;
        margin: 0;
        padding: 0;
    }

    .titulo-do-anuncio a { /*Estilização do link de compra e o titulo do anuncio*/
        text-align: center;
        width: 330px;
        padding: 20px;
        height: auto;
        font-size: 20pt;
        text-decoration: none;
        color:#f2f2f2;
        font-weight: 800;
        border-radius: 50px;
        background-color: #95E914;
        box-shadow: rgba(0, 0, 0, 0.17) 0px -23px 25px 0px inset, rgba(0, 0, 0, 0.15) 0px -36px 30px 0px inset, rgba(0, 0, 0, 0.1) 0px -79px 40px 0px inset, rgba(0, 0, 0, 0.06) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
    }

    #contador-promocional { /*Estilização do contador promocional */
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-template-rows: auto;
        align-items: center;
        justify-content: center;
        width: 450px;
        height: auto;
        margin: 0 auto;
        border-radius: 4px 125px 4px 125px;
        border-bottom: 5px solid #f2f2f294;
        border-top: 5px solid #f2f2f294;
        box-shadow: rgba(0, 0, 0, 0.17) 0px -23px 25px 0px inset, rgba(0, 0, 0, 0.15) 0px -36px 30px 0px inset, rgba(0, 0, 0, 0.1) 0px -79px 40px 0px inset, rgba(0, 0, 0, 0.06) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
    }
    
    #contador-promocional span { /*Estilização do contador promocional */
        align-items: center;
        justify-content: center;
        text-align: center;
        width: 105px;
        height: auto;   
        margin: 0 auto;
    }

    #contador-promocional small { /*Estilização do contador promocional */
        font-size: 10pt;
    }

    #contador-promocional p { /*Estilização do contador promocional */
        border: 1px solid #f2f2f294;
        border-radius: 4px;
        font-size: 50pt;
        font-weight: 500;
        border-radius: 25px;
        margin: 0;
        padding: 0;
    }

    #contador-promocional p:hover { /*Efeito de hover no contador promocional */
        background-color: #f2f2f294;
        color: #0D0D0D;
        transition: 0.3s ease-in-out;
    }

    .feedbacks-leitores { /*Estilização do container de feedbacks dos leitores */
        display: grid;
        align-items: center;
        justify-content: center;
        grid-template-rows: repeat(2, auto);    
        max-width: 1200px;
        width: 100vh;
        height: auto;
        margin: 0 auto;
        padding-top: 80px;
        padding-bottom: 80px;
    }

    .mensagem-representativa { /*Estilização da mensagem representativa */
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: center;
        width: 650px;
        height: auto;
        margin: 0 auto;
    }

    .mensagem-representativa h3 { /*Estilização do titulo da mensagem representativa */ 
        font-size: 40pt;
        font-weight: 900;
        margin: 0;
        padding: 0;
        color: #5b9208
    }

    .opnioes-leitores { /*Estilização do container de opnioes dos leitores */
        display: grid;
        grid-template-columns: repeat(3, auto);
        grid-template-rows: auto;
        width: 100%;
        height: auto;
        margin: 0 auto;
        padding-top: 75px;
    }

    .opnioes-leitores span { /*Estilização do container de opnioes dos leitores */
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 350px;
        height: 400px;
        margin: 0 auto;
        padding: 25px;
        border-top: solid 1px #f2f2f22d;
        border-bottom: solid 1px #f2f2f22d;    
        border-radius: 12px 0px 12px;
        
    }

    .opnioes-leitores span:hover { /*Efeito de hover no container de opnioes dos leitores */
        transition: 0.5s ease-in;
        background-color: #f2f2f207;
        transform: scale(1.05);
    }

    .ebook { /*Estilização do container da descrição do autor do ebook */
        display: flex;
        flex-direction: row;
        max-width: 1200px;
        width: 100vw;
        height: auto;
        margin: 0 auto;
        padding-top: 80px;
        padding-bottom: 80px;
        
    }

    .descricao-livro { /*Estilização da secao da descricao do autor */
        display: flex;
        flex-direction: column;
        width: 590px;
        height: auto;
        margin: 0 auto;
    }

    .descricao-livro h3 { /*Aumento do nivel de titulo para estilização. */
        font-size: 35pt;
        margin: 0;
    }

    .descricao-livro small {
        font-weight: 300;
    }

    .descricao-livro p {
        padding: 30px 0;
    }

    .fotografia-livro { /*Estilização do container da fotografia do autor*/
        display: flex;
        align-items: center;
        justify-content: right;
        width: 450px;
        height: auto;
    }

    .fotografia-livro img { /*Estilização e corte da foto do autor dos ebooks */
        width: 450px;
        height: auto;
        border-radius: 112px 0px 112px;
       
    }

    .sobre-autor { /*Estilização do container sobre o autor do ebook */
        display: grid;
        grid-template-columns: 1fr 1fr;
        max-width: 1200px;
        width: 100vw;
        height: auto;
        margin-bottom: 45px;
        padding-top: 80px;
        padding-bottom: 80px;
        background-color: #0D0D0D;
        border-radius: 112px 0px 112px;
    }

    .descricao-autor h3 { 
        font-size: 35pt;
        margin: 0;
    }

    .descricao-autor small {
        font-weight: 200;
    }

    .descricao-autor p {
        padding: 30px 0;
    }

    .descricao-autor { /*Dimensionamento e posicionamento da descrição do autor*/
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 490px;
        height: auto;
        margin: 0 auto;        
    }

    .fotografia-do-autor { /*Estilização do container da descrição do autor */
        display: flex;
        align-items: center;
        justify-content: right;
        width: 550px;
        height: auto;
    }

    .fotografia-do-autor img { /*Formatção da imagem do autor*/
        width: 450px;
        height: auto;
        border-radius: 50%;
        border: solid 2px #f2f2f2;
    }

    footer { /*Estilização do rodapé, container */
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        width: 100vw;
        height: 12rem;
        padding: 35px 0;
        background-color: #0D0D0D;
        
    }

    .links-rodape { /*Estilização do container dos links do rodapé */
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 650px;
        height: 92px;
    }

    .links-rodape h2 {
        font-size: 35pt;
    }

    .links-rodape p { /*Estilização do texto do rodape */
        font-size: 25pt;
        font-weight: 500;
        color: #f2f2f2e5;
        margin: 0;
    }

    .links-rodape small { /*Estilização do texto pequeno do rodapé */
        color: #f2f2f29c;
        font-weight: 200;
        margin-top: 45px;
    }

    .links-rodape nav { /*Estilização da tag de navegação dos links do rodape */
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        width: 100%;
        height: auto;

    }

    .others-links a {
        padding:  0 25px;
        color: #f2f2f29c;
        text-decoration: none;
    }   




    /*********RESPONSIVIDADE**********/

    @media (max-width: 1120px) {



        /******CABEÇALHO*******/
        header {
           width: 100vw;
        }

        header ul {
            display: none;
        }
        


        /****BANNER DO VIDEO DE APRESENTAÇÃO*******/
        .article {
            width: 75vw;

        }
        .introducao-ao-conteudo {
            flex-direction: column;
        }
        .banner-video {
            width: 75vw;
            height: 40vw;
        }
        .banner-video iframe {
            width: 75vw;
            height: 35vw;
        }
        .sobre-video {
          width: 75vw;
          height: 40vw;
          margin: 0 auto;
          text-align: left;
          
        }
        .sobre-video h1 {
            font-size: 35pt;
        }


        /****CONTAINER DE PROMOCAO E DESCONTOS*******/
        .promocao-desconto {
            flex-direction: column;
            width: 85vw;

        }
        .titulo-do-anuncio {
            text-align: center;
            width: 45vw;
            height: 30vw;
        }
        .titulo-do-anuncio a {
            width: 50vh;
        }
        #contador-promocional {
            width: 45vw;
            height: 20vw;
            border: none;
            background-color: none;
            box-shadow: none;
        }
        #contador-promocional p {
            font-size: 30pt;
        }


        /****FEEDBACKS DOS LEITORES******/
        .feedbacks-leitores {
            width: 75vw;
        }
        .mensagem-representativa {
            width: 50vw;
        }
     
        .opnioes-leitores {
            justify-content: center;
            width: 45vw;
            height: 100vw
        }
        .opnioes-leitores span {
            width: 30vw;
            height: 65vh;   
        }

        


        /*****SECAO DO LIVRO******/
        .ebook {
            width: 75vw; 
            height: 55vh;   
        }

        .descricao-livro { /*Responsividade da secao da descricao do autor */
            display: flex;
            flex-direction: column;
            justify-content: center;
            width: 50vw;
            height: 35vw;
            margin: 0 auto;
        }
        .fotografia-livro {
            align-items: center;
            justify-content: center;
            width: 45vw;
            height: 35vh;
        }
        .fotografia-livro img { /*Estilização e corte da foto do autor dos ebooks */
            width: 30vw;            
        }


        /***SOBRE O AUTO****/
        .sobre-autor {
            flex-direction: row;
            
            
        }
        .descricao-autor {
            width: 35vw;
        }
        .fotografia-do-autor {
            width: 45vw;
        }
    


        /*****RODAPE DO SITE*******/
        footer {
            width: 100vw;
            height: 35vh;
            margin: 0 auto;

            background-color: #0D0D0D;
            
        }
        .links-rodape h2 {
            font-size: 25pt;
        }
        .links-rodape p {
            font-size: 15pt;
        }
        
    }

    @media (max-width: 1120px) {

        /******CABEÇALHO*******/
        header {
           
           width: 100vw;
        }

        .logotipo {
            width: 75vw;
        }

        header ul {
            display: none;
        }

        #abrir-menu {
            display: flex;
            
        }   


        


        /****BANNER DO VIDEO DE APRESENTAÇÃO*******/
        .article {
            width: 75vw;

        }
        .introducao-ao-conteudo {
            flex-direction: column;
        }
        .banner-video {
            width: 75vw;
            height: 40vw;
        }
        .banner-video iframe {
            width: 75vw;
            height: 35vw;
        }
        .sobre-video {
          width: 75vw;
          height: 40vw;
          margin: 0 auto;
          text-align: left;
          
        }
        .sobre-video h1 {
            font-size: 35pt;
        }


        /****CONTAINER DE PROMOCAO E DESCONTOS*******/
        .promocao-desconto {
            flex-direction: column;
            width: 85vw;

        }
        .titulo-do-anuncio {
            text-align: center;
            width: 45vw;
            height: 30vw;
        }
        .titulo-do-anuncio a {
            width: 50vh;
        }
        #contador-promocional {
            width: 45vw;
            height: 20vw;
            border: none;
            background-color: none;
            box-shadow: none;
        }

        #contador-promocional p {
            font-size: 30pt;
        }


        /****FEEDBACKS DOS LEITORES******/
        .feedbacks-leitores {
            width: 75vw;
        }
        .mensagem-representativa {
            width: 50vw;
        }
        .opnioes-leitores {
            justify-content: center;
            width: 45vw;
            height: 100vw
        }
        .opnioes-leitores span {
            width: 30vw;
            height: 65vh;   
        }

        


        /*****SECAO DO LIVRO******/
        .ebook {
            width: 75vw; 
            height: 55vh;   
        }

        .descricao-livro { /*Responsividade da secao da descricao do autor */
            display: flex;
            flex-direction: column;
            justify-content: center;
            width: 50vw;
            height: 35vw;
            margin: 0 auto;
        }
        .fotografia-livro {
            align-items: center;
            justify-content: center;
            width: 45vw;
            height: 35vh;
        }
        .fotografia-livro img { /*Estilização e corte da foto do autor dos ebooks */
            width: 30vw;            
        }


        /***SOBRE O AUTO****/
        .sobre-autor {
            flex-direction: row;
            
            
        }
        .descricao-autor {
            width: 35vw;
        }
        .fotografia-do-autor {
            width: 45vw;
        }


        /*****RODAPE DO SITE*******/
        footer {
            width: 100vw;
            height: 35vh;
            margin: 0 auto;

            background-color: #0D0D0D;
            
        }
        .links-rodape h2 {
            font-size: 25pt;
        }
        .links-rodape p {
            font-size: 15pt;
        }
        
    }

    @media (max-width: 922px) {

        /******CABEÇALHO*******/
        header {
        width: 100vw;
        }

        .logotipo {
            width: 75vw;
        }

        header ul {
            display: none;
        }

        #abrir-menu {
            display: flex;
        }



        /****BANNER DO VIDEO DE APRESENTAÇÃO*******/
        .article {
            width: 75vw;

        }
        .introducao-ao-conteudo {
            flex-direction: column;
        }
        .banner-video {
            width: 75vw;
            height: 40vw;
        }
        .banner-video iframe {
            width: 75vw;
            height: 35vw;
        }
        .sobre-video {
            width: 75vw;
            height: 40vw;
            margin: 0 auto;
            text-align: left;
        
        }
        .sobre-video h1 {
            font-size: 35pt;
        }


        /****CONTAINER DE PROMOCAO E DESCONTOS*******/
        .promocao-desconto {
            flex-direction: column;
            width: 85vw;
            height: 85vw;

        }
        .titulo-do-anuncio {
            text-align: center;
            width: 45vw;        
            height: 60vw;
        }
        .titulo-do-anuncio a {
            width: 50vh;
        }
        #contador-promocional {                                                                                                                                                         
            width: 45vw;
            height: 40vw;
            border: none;
            background-color: none;
            box-shadow: none;
        }

        #contador-promocional p {
            font-size: 30pt;
        }


        /****FEEDBACKS DOS LEITORES******/
        .feedbacks-leitores {
            display: none;
            width: 75vw;
        }
        .mensagem-representativa {
            width: 50vw;
            height: 50vw;
        }

        .opnioes-leitores {
            display: none;  
            justify-content: center;
            width: 45vw;
            height: 100vw;
        }
        .opnioes-leitores span {
            width: 30vw;
            height: 65vh;   
        }




        /*****SECAO DO LIVRO******/
        .ebook {
            width: 100vw; 
            height: 50vh;   
        }

        .descricao-livro { /*Responsividade da secao da descricao do autor */
            display: flex;
            flex-direction: column;
            justify-content: center;
            width: 75vw;
            height: 50vw;
            margin: 0 auto;
        }
        .fotografia-livro {
            display: none;
            align-items: center;
            justify-content: center;
            width: 45vh;
            height: 35vh;
        }
        .fotografia-livro img { /*Estilização e corte da foto do autor dos ebooks */
            width: 20px;            
        }


        /***SOBRE O AUTO****/
        .sobre-autor {
            flex-direction: row;
            
            
        }
        .descricao-autor {
            width: 35vw;
        }
        .fotografia-do-autor {  
            width: 45vw;
        }
        .fotografia-do-autor img {
            width: 25vh;
        }


        /*****RODAPE DO SITE*******/
        footer {
            width: 100vw;
            height: 35vh;
            margin: 0 auto;

            background-color: #0D0D0D;
            
        }
  
        .links-rodape h2 {
            font-size: 25pt;
        }
        .links-rodape p {
            font-size: 15pt;
        }

    }

    @media (max-width: 760px) {


    /******CABEÇALHO*******/
    header {
    width: 100vw;
    }

    .logotipo {
        width: 75vw;
    }

    header ul {
        display: none;
    }

    #abrir-menu {
        display: flex;
    }

    


    /****BANNER DO VIDEO DE APRESENTAÇÃO*******/
    .article {
        width: 75vw;

    }
    .introducao-ao-conteudo {
        flex-direction: column;
    }
    .banner-video {
        width: 75vw;
        height: 40vw;
    }
    .banner-video iframe {
        width: 75vw;
        height: 35vw;
    }
    .sobre-video {
        width: 75vw;
        height: 75vw;
        margin: 0 auto;
        text-align: left;
    
    }
    .sobre-video h1 {
        font-size: 35pt;
    }


    /****CONTAINER DE PROMOCAO E DESCONTOS*******/
    .promocao-desconto {
        flex-direction: column;
        width: 100vw;
        height: 100vh;

    }
    .titulo-do-anuncio {
        text-align: center;
        width: 75vw;        
        height: 100vw;
    }
    .titulo-do-anuncio a {
        width: 100vh;
    }
    #contador-promocional {                                                                                                                                                         
        width: 75vw;
        height: 40vw;
        border: none;
        background-color: none;
        box-shadow: none;
    }
    #contador-promocional p {
        font-size: 30pt;
    }


    /****FEEDBACKS DOS LEITORES******/
    .feedbacks-leitores {
        display: none;
        width: 75vw;
    }
    .mensagem-representativa {
        width: 50vw;
        height: 50vw;
    }

    .opnioes-leitores {
        display: none;  
        justify-content: center;
        width: 45vw;
        height: 100vw;
    }
    .opnioes-leitores span {
        width: 30vw;
        height: 65vh;   
    }




    /*****SECAO DO LIVRO******/
    .ebook {
        width: 100vw; 
        height: 100vh;   
    }

    .descricao-livro { /*Responsividade da secao da descricao do autor */
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 90vw;
        height: 100vw;
        margin: 0 auto;
    }
    .fotografia-livro {
        display: none;
        align-items: center;
        justify-content: center;
        width: 45vh;
        height: 35vh;
    }
    .fotografia-livro img { /*Estilização e corte da foto do autor dos ebooks */
        width: 20px;            
    }


    /***SOBRE O AUTO****/
    .sobre-autor {
        display: flex;
        flex-direction: row;
        width: 100vw;
        height: 100vw;

    }
    .descricao-autor {
        
        width: 75vw;
    }
    .fotografia-do-autor {
        display: none;  
        width: 45vw;
    }



    /*****RODAPE DO SITE*******/
    footer {
        width: 100vw;
        height: 35vh;
        margin: 0 auto;

        background-color: #0D0D0D;
        
    }

    .links-rodape h2 {
        font-size: 25pt;
    }
    .links-rodape p {
        font-size: 15pt;
    }

}

    @media (max-width: 550px) {


/****CONTAINER PRINCIPAL****/


    /******CABEÇALHO*******/
    header {
    width: 100vw;
    }

    .logotipo {
        width: 75vw;
    }

    header ul {
        display: none;
    }

    #abrir-menu {
        display: flex;
    }



    /****BANNER DO VIDEO DE APRESENTAÇÃO*******/
    .article {
        width: 75vw;

    }
    .introducao-ao-conteudo {
        flex-direction: column;
    }
    .banner-video {
        width: 75vw;
        height: 40vw;
    }
    .banner-video iframe {
        width: 75vw;
        height: 35vw;
    }
    .sobre-video {
        width: 75vw;
        height: 75vw;
        margin: 0 auto;
        text-align: left;
    
    }
    .sobre-video h1 {
        font-size: 35pt;
    }


    /****CONTAINER DE PROMOCAO E DESCONTOS*******/
    .promocao-desconto {
        flex-direction: column;
        width: 100vw;
        height: 100vh;

    }
    .titulo-do-anuncio {
        text-align: center;
        width: 85vw;        
        height: 100vw;
    }
    .titulo-do-anuncio h1 {
        font-size: 15pt;
    }
    .titulo-do-anuncio a {
        width: 100vh;
        font-size: 13pt;
    }
    #contador-promocional {                                                                                                                                                         
        width: 75vw;
        height: 100vw;
        border: none;
        background-color: none;
        box-shadow: none;
    }
  
    #contador-promocional p {
        font-size: 30pt;
    }


    /****FEEDBACKS DOS LEITORES******/
    .feedbacks-leitores {
        display: none;
        width: 75vw;
    }
    .mensagem-representativa {
        width: 50vw;
        height: 50vw;
    }

    .opnioes-leitores {
        display: none;  
        justify-content: center;
        width: 45vw;
        height: 100vw;
    }
    .opnioes-leitores span {
        width: 30vw;
        height: 65vh;   
    }




    /*****SECAO DO LIVRO******/
    .ebook {
        width: 100vw; 
        height: 100vh;   
    }

    .descricao-livro { /*Responsividade da secao da descricao do autor */
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 90vw;
        height: 100vh;
        margin: 0 auto;
    }
    .fotografia-livro {
        display: none;
        align-items: center;
        justify-content: center;
        width: 45vh;
        height: 35vh;
    }
    .fotografia-livro img { /*Estilização e corte da foto do autor dos ebooks */
        width: 20px;            
    }


    /***SOBRE O AUTO****/
    .sobre-autor {
        display: flex;
        flex-direction: row;
        width: 100vw;
        height: 100vh;

    }
    .descricao-autor {
        
        width: 75vw;
    }
    .fotografia-do-autor {
        display: none;  
        width: 45vw;
    }
 

    /*****RODAPE DO SITE*******/
    footer {
        width: 100vw;
        height: 35vh;
        margin: 0 auto;

        background-color: #0D0D0D;
        
    }
  
    .links-rodape h2 {
        font-size: 25pt;
    }
    .links-rodape p {
        font-size: 15pt;
    }
}

@media (max-width: 490px) {


/****CONTAINER PRINCIPAL****/


    /******CABEÇALHO*******/
    header {
    width: 100vw;
    }

    .logotipo {
        width: 75vw;
    }

    header ul {
        display: none;
    }

    #abrir-menu {
        display: flex;
    }



    /****BANNER DO VIDEO DE APRESENTAÇÃO*******/
    .article {
        width: 75vw;

    }
    .introducao-ao-conteudo {
        flex-direction: column;
    }
    .banner-video {
        width: 75vw;
        height: 40vw;
    }
    .banner-video iframe {
        width: 75vw;
        height: 35vw;
    }
    .sobre-video {
        width: 75vw;
        height: 75vw;
        margin: 0 auto;
        text-align: left;
    
    }
    .sobre-video h1 {
        font-size: 20pt;
    }


    /****CONTAINER DE PROMOCAO E DESCONTOS*******/
    .promocao-desconto {
        flex-direction: column;
        width: 100vw;
        height: 100vh;

    }
    .titulo-do-anuncio {
        text-align: center;
        width: 85vw;        
        height: 100vw;
    }
    .titulo-do-anuncio h1 {
        font-size: 15pt;
    }
    .titulo-do-anuncio a {
        width: 100vh;
        font-size: 13pt;
    }
    #contador-promocional {                                                                                                                                                         
        width: 75vw;
        height: 100vw;
        border: none;
        background-color: none;
        box-shadow: none;
    }

    #contador-promocional p {
        font-size: 30pt;
    }


    /****FEEDBACKS DOS LEITORES******/
    .feedbacks-leitores {
        display: none;
        width: 75vw;
    }
    .mensagem-representativa {
        width: 50vw;
        height: 50vw;
    }
 
    .opnioes-leitores {
        display: none;  
        justify-content: center;
        width: 45vw;
        height: 100vw;
    }
    .opnioes-leitores span {
        width: 30vw;
        height: 65vh;   
    }




    /*****SECAO DO LIVRO******/
    .ebook {
        align-items: center;
        width: 100vw; 
        height: 100vh;   
    }

    .descricao-livro { /*Responsividade da secao da descricao do autor */
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 90vw;
        height: 100vw;
        margin: 0 auto;
    }
    .descricao-livro h3 {
        font-size: 25pt;
    }
    .fotografia-livro {
        display: none;
        align-items: center;
        justify-content: center;
        width: 45vh;
        height: 35vh;
    }
    .fotografia-livro img { /*Estilização e corte da foto do autor dos ebooks */
        width: 20px;            
    }


    /***SOBRE O AUTO****/
    .sobre-autor {
        display: flex;
        flex-direction: row;
        width: 100vw;
        height: 100vh;

    }
    .descricao-autor {
        width: 75vw;
    }
    .fotografia-do-autor {
        display: none;  
        width: 45vw;
    }



    /*****RODAPE DO SITE*******/
    footer {
        width: 100vw;
        height: 35vh;
        margin: 0 auto;

        background-color: #0D0D0D;
        
    }

    .links-rodape h2 {
        font-size: 25pt;
    }
    .links-rodape p {
        font-size: 15pt;
    }
}

@media (max-width: 420px) {


/****CONTAINER PRINCIPAL****/


    /******CABEÇALHO*******/
    header {
    width: 100vw;
    }

    .logotipo {
        width: 75vw;
    }

    header ul {
        display: none;
    }

    #abrir-menu {
        display: flex;
    }



    /****BANNER DO VIDEO DE APRESENTAÇÃO*******/
    .article {
        width: 75vw;

    }
    .introducao-ao-conteudo {
        flex-direction: column;
    }
    .banner-video {
        width: 75vw;
        height: 75vw;
    }
    .banner-video iframe {
        width: 100vw;
        height: 55vw;
    }
    .sobre-video {
        width: 75vw;
        height: 50vh;
        margin: 0 auto;
        text-align: left;
    
    }
    .sobre-video h1 {
        font-size: 15pt;
    }


    /****CONTAINER DE PROMOCAO E DESCONTOS*******/
    .promocao-desconto {
        flex-direction: column;
        width: 100vw;
        height: 100vh;

    }
    .titulo-do-anuncio {
        text-align: center;
        width: 85vw;        
        height: 100vw;
    }
    .titulo-do-anuncio h1 {
        font-size: 15pt;
    }
    .titulo-do-anuncio a {
        width: 100vh;
        font-size: 13pt;
    }
    #contador-promocional {                                                                                                                                                         
        width: 75vw;
        height: 100vw;
        border: none;
        background-color: none;
        box-shadow: none;
    }

    #contador-promocional p {
        font-size: 30pt;
    }


    /****FEEDBACKS DOS LEITORES******/
    .feedbacks-leitores {
        display: none;
        width: 75vw;
    }
    .mensagem-representativa {
        width: 50vw;
        height: 50vw;
    }

    .opnioes-leitores {
        display: none;  
        justify-content: center;
        width: 45vw;
        height: 100vw;
    }
    .opnioes-leitores span {
        width: 30vw;
        height: 65vh;   
    }




    /*****SECAO DO LIVRO******/
    .ebook {
        align-items: center;
        width: 100vw; 
        height: 100vh;   
    }

    .descricao-livro { /*Responsividade da secao da descricao do autor */
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 90vw;
        height: 100vh;
        margin: 0 auto;
    }
    .descricao-livro h3 {
        font-size: 25pt;
    }
    .fotografia-livro {
        display: none;
        align-items: center;
        justify-content: center;
        width: 45vh;
        height: 35vh;
    }
    .fotografia-livro img { /*Estilização e corte da foto do autor dos ebooks */
        width: 20px;            
    }


    /***SOBRE O AUTO****/
    .sobre-autor {
        display: flex;
        flex-direction: row;
        width: 100vw;
        height: 100 vh;

    }
    .descricao-autor {
        width: 75vw;
    }
    .fotografia-do-autor {
        display: none;  
        width: 45vw;
    }
 


    /*****RODAPE DO SITE*******/
    footer {
        width: 100vw;
        height: 45vh;
        margin: 0 auto;

        background-color: #0D0D0D;
        
    }

    .links-rodape h2 {
        font-size: 25pt;
    }
    .links-rodape p {
        font-size: 15pt;
    }
}
</style>
