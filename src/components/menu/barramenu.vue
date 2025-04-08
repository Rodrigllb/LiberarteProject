<template>
         
        <header>

            <div class="logotipo">
                <img src="../../assets/logo-liberarte.png" alt="logo liberarte">
            </div>

            <nav>
                <ul>
                    <li><a href="#">Nossos Livros</a></li>
                    <li><a href="https://wa.link/9cg7g0" target="_blank">Whatsapp</a></li>
                    <li><a href="#sobre">Sobre</a></li>
                    <li><a id="link-buy" href="https://go.hotmart.com/F98346505C?dp=1" target="_blank">COMPRE AGORA</a></li>
                </ul>
            </nav>

            <button id="abrir-menu"><img src="../../assets/icon-menu.png" alt="botão para abrir menu"></button>
            
        </header>
        <div id="menu-aberto">
                <h2>Outras obras</h2>
                <small>Conheça mais das obras de José Liberato!</small>
                <ul>
                    <li><a href="https://go.hotmart.com/E98661529C" target="_blank" rel="noopener noreferrer">Do Caos À Calma</a></li>
                    <li><a href="https://go.hotmart.com/M98772478S" target="_blank" rel="noopener noreferrer">A força Invísivel</a></li>
                    <li><a href="https://go.hotmart.com/F98346505C?dp=1" target="_blank" rel="noopener noreferrer">Tudo Começa Em Você</a></li>
                </ul>
                <h2>Redes Sociais</h2>
                <ul>
                    <li><a href="https://www.instagram.com/jose.railson22?igsh=ODI5Z3ZqNGE0cjE4" target="_blank" rel="noopener noreferrer"><img src="./../../assets/icon-insta.png" alt="instagram"> Instagram</a></li>
                    <li><a href="https://wa.link/9cg7g0" target="_blank" rel="noopener noreferrer"><img src="./../../assets/icon-wpp.png" alt="whatsapp"> Whatsapp</a></li>
                </ul>
               
                    
        </div>
  
  
</template>


<script>
export default {
    name: 'barraMenu',
}


//Somente carregar o código quando o DOM do js for carregado completamente.
document.addEventListener('DOMContentLoaded', function domLoaded() {
    const execMenu = document.getElementById('abrir-menu') ; //Coleto o botão
    const menuExec = document.getElementById('menu-aberto'); //Coleto o menu

    if(execMenu) { //Verifico se os elementos estão carregado corretamente para não have conflitos.
        execMenu.addEventListener('click', function abrirMenu(){
            if(menuExec.style.display === 'none' || menuExec.style.display === '') {
                menuExec.style.display = 'flex';
                console.log('arquivo carregado');
            }
            else {
                menuExec.style.display = 'none';
                
            }
        });
    }
    else { //Senão estão, o mesmo é lançado uma mensagem de erro no console.
        console.error('elemento não carregado');
    }
});






</script>

<style scoped>

    header { /*Estilização do cabeçalho */
        display: flex;
        justify-content: center;
        align-items: center;
        position: sticky;
        top: 0;
        width: 100vw;
        height: 10vh;
        margin: 0 auto;
        background-color: #0D0D0D;
        box-shadow: rgba(0, 0, 0, 0.45) 0px 25px 20px -20px;
    }

    header a { /*Padronização dos links no cabeçalho */
        text-decoration: none;
        color: #F2F2F2;
    }

    header ul { /*Estilização da lista para poscionamento dos links no cabeçalho */
        display: flex;
        flex-direction: row;
        justify-content: right;
        list-style: none;
        margin: 0 45px;
    }

    header li { /*Estilização dos itens da lista */
        margin: 0 55px;
    }

    #link-buy { /*Link de compra*/
        text-align: center;
        font-weight: 500;
        color: #95E914;
    }

    #link-buy:hover { /*Efeito de hover no link de compra */
        background-color: #95E914;
        color: #0D0D0D;
        transition: 0.3s ease-in-out;
    }

    #abrir-menu { /*Estilização do icone de menu */
        display: none;
        background: none;
        border: none;
    }

    #menu-aberto {
        transition: 0.5s ease;
        display: none;
        position: fixed;
        align-content: center;
        flex-direction: column; 
        padding: 25px;
        background-color: #f2f2f2;
        color: #0D0D0D;
        width: 100vw;
        height: 45vh;
        box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
    }

    #menu-aberto .logoLA {
        width: 105px;
        height: auto;
    }

    #menu-aberto h2, small {
        padding: 0; 
        margin: 0;
        font-weight: 200;
    }

    #menu-aberto a, ul {
        color: #0D0D0D;
        list-style: none;
        text-decoration: none;
    }






    /****RESPONSIVIDADE*****/
    @media (max-width: 1120px) {




        /******CABEÇALHO*******/
        header {
        width: 100vw;
        }

        header ul {
            display: none;
        }

    }


    @media (max-width: 1120px) {


        /****CONTAINER PRINCIPAL****/
        #container-principal {  
            
        }


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
    }

    @media (max-width: 922px) {


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

    }

    @media (max-width: 760px) {


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

    }



</style>