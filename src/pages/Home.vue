<template>
  <Header/>
      <section>
            <div class="Slider-containner">
                <div id="Slider" class="carousel slide" data-ride="carousel">
                    <ol class="carousel-indicators">
                        <li data-target="#Slider" data-slide-to="0" class="active"></li>
                        <li data-target="#Slider" data-slide-to="1"></li>
                    </ol>
                    <div class="carousel-inner">
                        <div class="carousel-item active">
                          <img class="d-block" src="../images/icons/Slider.png" alt="First slide">
                        </div>
                        <div class="carousel-item">
                          <img class="d-block" src="../images/icons/Slider1.png" alt="Second slide">
                        </div>
                    </div>
                    <a class="carousel-control-prev w-80" href="#Slider" role="button" data-slide="prev">
                        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                        <span class="sr-only">Previous</span>
                    </a>
                    <a class="carousel-control-next w-80" href="#Slider" role="button" data-slide="next">
                        <span class="carousel-control-next-icon" aria-hidden="true"></span>
                        <span class="sr-only">Next</span>
                    </a>
                </div>  
            </div>
        </section>
        <!--Corpo-->
        <section class="section">
            <!--Menu 2-->
            <div class="menu2">
                <div class="containner">
                    <div class="section">
                        <a href="lista.html"><img src="../images/icons/icon_processadores.png" alt="processadores"></a>
                        <div class="texto">
                            <a href="lista.html">Processadores</a>
                        </div>
                    </div>
                    <div class="section">
                        <div class="icon">
                            <a href="#"><img src="../images/icons/icon_placavideo.png" alt="processadores"></a>
                        </div>
                        <div class="texto">
                            <a href="#">Placa de vídeo</a>
                        </div>
                    </div>
                    <div class="section">
                        <div class="icon">
                            <a href="#"><img src="../images/icons/icon_memoria.png" alt="processadores"></a>
                        </div>
                        <div class="texto">
                            <a href="#">Memória RAM</a>
                        </div>
                    </div>
                    <div class="section">
                        <div class="icon">
                            <a href="#"><img src="../images/icons/icon_hdssd.png" alt="processadores"></a>
                        </div>
                        <div class="texto">
                            <a href="#">HD/SSD</a>
                        </div>
                    </div>
                    <div class="section">
                        <div class="icon">
                            <a href="#"><img src="../images/icons/icon_monitor.png" alt="processadores"></a>
                        </div>
                        <div class="texto">
                            <a href="#">Monitor</a>
                        </div>
                    </div>
                    <div class="section">
                        <div class="icon">
                            <a href="#"><img src="../images/icons/icon_acessorios.png" alt="processadores"></a>
                        </div>
                        <div class="texto">
                            <a href="#">Acessórios</a>
                        </div>
                    </div>
                </div>
            </div>
            <!--1° bloco-->
            <div class="containner"> 
                <div class="bloco">
                    <img class="../images/icons-fluid grow img-shadow" src="../images/icons/processadores_amd_intel.png">
                    <div class="paragrafo">
                        <div>
                            <span>
                                <h4><b>PROCESSADORES</b> | ALTA PERFORMACE</h4>
                                <p>Alta resolução em um monitor, a experiência visual é extremamente realista.
                                    Jogue com configuração no ultra e veja seus filmes preferidos com qualidade de cinema. 
                                </p>
                                <a href="lista.html"><h6>Veja mais produtos</h6></a>
                            </span>
                        </div>
                    </div>
                </div>
                <!--Bloco do meio-->
                <div class="bloco_do_meio">
                    <div class="bloco">
                        <img class="../images/icons-fluid grow img-shadow img_resp" src="../images/icons/memorias.png">
                        <div class="paragrafo">
                            <div>
                                <span>
                                    <h4><b>SSD</b> | AGILIDADE EM TAREFAS BÁSICAS</h4>    
                                    <p>Tecnologia de resposta inteligente combina o rápido desempenho de uma pequena
                                        unidade de estado sólido com a alta capacidade de um disco rígido.
                                    </p>
                                    <a href="#"><h6>Veja mais produtos</h6></a>
                                </span>
                            </div>
                        </div>
                        <img class="../images/icons-fluid grow img-shadow img" src="../images/icons/memorias.png">
                    </div>
                </div>
                <!--Ultimo bloco-->
                <div class="bloco">
                    <img class="../images/icons-fluid grow img-shadow" src="../images/icons/monitor.png">
                    <div class="paragrafo">
                        <div>
                            <span>
                                <h4><b>MONITORES</b> | ALTA RESOLUÇÃO</h4>
                                <p>Alta resolução em um monitor, a experiência visual é extremamente realista.
                                    Jogue com configuração no ultra e veja seus filmes preferidos com qualidade de cinema. 
                                </p>
                                <a href="#"><h6>Veja mais produtos</h6></a>
                            </span>
                        </div>
                    </div>
                </div>
            </div>
        </section>
  
    <Footer/>

</template>

<script>

import 'bootstrap/dist/css/bootstrap.min.css'
import 'bootstrap/dist/js/bootstrap.min.js'


import Header from "../components/Header.vue";
import Footer from "../components/Footer.vue";



export default {
  name: "Home",

  components:{
      Header, 
      Footer
  }
  
};
</script>

<style>
/* Nao esquecer de colocar ; no final do @import */
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:ital,wght@0,300;0,400;0,600;0,700;1,300;1,400&display=swap');


/*Geral*/
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    outline: 0;
  }
html {
    font-size: 100%;
}
body, html{
    height: 100vh;
    font-family: 'Source Sans Pro', sans-serif;
    text-rendering: optimizelegibility;
    -webkit-font-smoothing: antialiased;
}
body {
    font-size: 1.6rem;
}
/*-------------------------------------------------------------------*/
/*************SLIDER**************/
/*imagens do corrocel (seguir padrao de tamanho 1902x714)*/
.carousel-inner img{
    position: relative;
    margin:auto;
    width: 100%;
    max-width: 1500px;
}
/*Coloca o corrocel para traz do menu*/
Section div .carousel {
    position: relative;
    z-index: 1;
}
/*indacador lateral direito do slider*/
section .carousel-control-prev-icon {
    width: 50px;
    height: 30px;
}
/*indacador lateral esquerdo do slider*/
section .carousel-control-next-icon {
    width: 50px;
    height: 30px; 
}
/*indicadores inferiores do slider*/
section .carousel-indicators li {
    width: 50px;
    height: 4px;
    background-color: rgb(0, 174, 255);
}
/*-------------------------------------------------------------------------*/
/*****************MENU 2****************/
/*Div principal*/
section .menu2 {
    position: relative;
    width: 100%;
    background-color: rgb(243, 243, 243);
    box-shadow: 0px 2px 5px rgb(172, 172, 172);
}
/*div-2 com largura do site (com grid 6 colunas 1 linha)*/ 
section .menu2 .containner {
    justify-content: space-between;
    width: 90%;
    max-width: 1200px;
    margin: auto;

    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
    grid-template-rows: 1fr;
}
/*div com itens dentro*/
section .menu2 .containner .section {
    padding: 20px;
}
/*div com icone*/
section .menu2 .containner .section  {
    position: relative;
    text-align: center;
}
/*imagem*/
section .menu2 .containner .section img {
    width: 40px;
}
/*div com link*/
section .menu2 .containner .section .texto {
    position: relative;
    padding-top: 10px;
}
/*link(texto)*/
section .menu2 .containner .section .texto a {
    text-decoration: none;
    color: rgb(70, 70, 70);
}
/*Hover da section*/
section .menu2 .containner .section:hover {
    background-color: rgb(255, 255, 255);
    box-shadow: rgb(43, 43, 43) 0px 0px 1px;
}
/*hover do texto*/
section .menu2 .containner .section .texto a:hover {
    color: rgb(128, 128, 128);
}
/*hover do icon*/
section .menu2 .containner .section a img:hover {
    filter: contrast(10%);
}
/*------------------------------------------------------------------------------*/
/*************Corpo do site, PROCESSADORES, MONITOR, MEMORIAS***************/
section .containner {
    width: 90%;
    max-width: 1200px;
    margin: auto;
}
/*Bloco do containner*/
section .containner .bloco{
    display: flex;
}
/*img do bloco*/
section .containner .bloco img {
    width: 500px;
    margin-top: 50px;
    margin-bottom: 50px;
}
/*bloco do paragrafo*/
section .containner .bloco .paragrafo {
    position: relative;
    display: block;
}
/*div do paragrafo*/
section .containner .bloco .paragrafo div {
    margin-top: 130px;
    margin-left: 150px; 
}
/*Paragrafos*/
section .containner .bloco .paragrafo div span {
    display: block;
}
/*"Veja mais" do paragrafo*/
section .containner .bloco .paragrafo div span h4{
    font-size: 1.1rem;
    font-weight: 400;
}
/*Tira sublinhado do link "veja mais" */
section .containner .bloco .paragrafo span a {
    text-decoration:none;
}
/*div do paragrafo do meio*/
section .containner .bloco_do_meio .bloco .paragrafo div {
    margin-top: 150px;
    margin-left: unset;
    margin-right: 50px;
}
/*posiciona img a direita do bloco do meio*/
section .containner .bloco_do_meio .bloco .img {
    width: 500px;
}
/*Img incia desativada e atiavada posteriormente na responsividade*/
section .containner .bloco_do_meio .bloco .img_resp {
    display: none;
}

/*Responsivo da página index*/
@media(max-width: 1075px) {
    section .containner .bloco .paragrafo div {
        margin-left: 100px; 
    }

    section .containner .bloco img {
        width: 400px;
    }

    section .containner .bloco_do_meio .bloco .paragrafo div {
        margin-right: unset;
    }
    section .containner .bloco_do_meio .bloco img {
        width: 400px;
    }
}

@media (max-width: 991px) {
    html {
        font-size: 95%;
    }

    section .bloco_do_meio .bloco .img{
        width: 400px;
    }
    
    section .bloco .paragrafo div{
        margin-left: 20px;
    }
}

@media (max-width: 790px) {
    section .containner .bloco {
        display: block;
        text-align: center;
        margin-bottom: 50px;
    }
    section .containner .bloco img {
        margin: 0;
        margin-top: 10px;  
    }
    section .containner .bloco .paragrafo div {
        margin: 0;
        margin-top: 40px;
    }
    section .containner .bloco .paragrafo div span {
        text-align: center;
    }
    section .containner .bloco_do_meio .bloco .paragrafo div {
        margin: 0;
        margin-top: 40px;
    }
    section .containner .bloco_do_meio .bloco .img {
        display: none;
    }
    section .containner .bloco_do_meio .bloco .img_resp {
        display: inline;
    }
    section .menu2 .containner {
        grid-template-columns: 1fr 1fr;
    }   
}

@media (max-width: 500px) {
    html {
        font-size: 85%;
    }
    section .containner .bloco img{
        width: 330px;
    }
    section .containner .bloco_do_meio .bloco img{
        width: 330px;
    }
}
@media (max-width: 320px) {
    html {
        font-size: 80%;
    }

    section .containner .bloco img{
        width: 80%;
    }
    section .containner .bloco_do_meio .bloco img{
        width: 80%;
    }
    .section .menu2 .containner .section{
        font-size: 80%;
    }


}
</style>
