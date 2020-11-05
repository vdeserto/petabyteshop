<template>
    <header>
            <!--div cabeçalho-->
            <div class="cabecalho">
                <!--NavBar-->
                <nav class="navbar navbar-expand-lg navbar-light bg-light">         
                    <!--botão toogle responsivo-->
                    <button onclick="clickNone()" class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                    <!--Logo 2- ativada somente na responsividade-->
                    <img class="logo2" src="../images/icons/logo2.png" alt="logo2">

                    <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
                        <!--Logo principal-->
                        <a class="navbar-brand" href="#"><img class="../images/icons-fluid grow logo" src="../images/icons/logo.png" alt="Petabyte SHOP"></a>
                        <!--Div com caixa de pesquisa e menu-lista-->
                        <div class="lista_form">
                            <!--Caixa de pesquisa-->
                            <form class="form-inline my-2 my-lg-0">
                                <input class="form-control mr-sm-2" type="search" placeholder="Buscar processadores memórias e muito mais!" aria-label="Search">
                                <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Buscar</button>
                            </form>
                            <!--Menu-lista-->
                            <ul class="navbar-nav mr-auto mt-2 mt-lg-0">
                                <li class="nav-item grow">
                                    <a class="nav-link" href="#">INÍCIO</a>
                                </li>
                                <li class="nav-item dropdown grow">
                                    <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                                        HARDWARES
                                    </a>
                                    <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
                                        <a class="dropdown-item" href="./lista.html">PROCESSADORES</a>
                                        <a class="dropdown-item" href="#">MEMÓRIAS</a>
                                        <a class="dropdown-item" href="#">PLACA DE VÍDEO</a>
                                        <a class="dropdown-item" href="#">PLACA MÃE</a>
                                        <a class="dropdown-item" href="#">HDD</a>
                                        <a class="dropdown-item" href="#">SSD</a>
                                    </div>
                                </li>
                                <li class="nav-item grow">
                                        <a class="nav-link" href="#">MONITORES</a>
                                </li>
                                <li class="nav-item grow">
                                    <a class="nav-link" href="#">ACESSÓRIOS</a>
                                </li>
                                <li class="nav-item grow">
                                    <a class="nav-link" href="#">PROMOÇÕES</a>
                                </li>
                                <li class="nav-item grow">
                                    <a class="nav-link" href="#">SOBRE</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <!--Login/carrinho-->
                    <div class="acesso" id="none">
                        <div>                           
                            <a href="./login.html"><img src="../images/icons/login.png"></a>
                            <a class="text" href="./login.html">Login</a>
                            <a href=""><img src="../images/icons/carrinho.png"></a>
                            <a class="text t2" href="">Carrinho</a>
                        </div>
                    </div>
                </nav>
            </div>
        </header>
</template>

<script>

export default
{
    name: "Header",
    
}
</script>

<style>
/********HEADER (LOGO, CAIXA DE PESQUISA, MENU/DROPDOWN e LOGIN/CARRINHO**********/
header {
    background-color: #f8f9fa!important;
}
/*div principal do header*/
header .cabecalho {
    position: relative;
    justify-content: space-between;
    width: 95%;
    max-width: 1200px;
    margin: auto; 
    z-index: 20; 
}
/*Logo*/
header .cabecalho a .logo {
    width: 160px;  
}
/*Logo 2- desativado (ativado na responsividade)*/
header .cabecalho .logo2 {
    display: none;
}
/*Nav emcima do slider*/
header .cabecalho nav {
    z-index: 10;
}
/*div com o menu e a caixa de pesquisa dentro alinhados em block*/
header .cabecalho nav .lista_form {
    display: block;
}
/*texto do menu*/
header .cabecalho nav .lista_form ul li a {
    font-size: 0.9rem;
    font-weight: 600;
}
/*botão buscar da caixa de pesquisa*/
header .cabecalho nav .lista_form form button {
    color: rgb(0, 110, 255);  
    border: rgb(0, 110, 255) solid 1px; 
    height: 30px;
    font-size: 0.9rem;
    padding-top: 2px;
}
/*hover do botão buscar da caixa de pesquisa*/
header .cabecalho nav .lista_form form button:hover {
    background-color: rgb(0, 110, 255);  
    color: white;

}
/*input da caixa de pesquisa*/
header .cabecalho nav .lista_form form input {
    font-size: 0.9rem;
    height: 30px;
    width: 45vw;
    max-width: 700px;


}
/*usado para na função clickNone para desativar/ativar a div login/carrinho*/
#none {
    display: inline;
}
/*alinhando login/carrinho*/
header .cabecalho .acesso {
    margin-bottom: auto;
}
/*Img login/carrinho*/
header .cabecalho .acesso div a img {
    width: 20px;
}
/*Texto da lista login/carrinho*/
header .cabecalho .acesso div .text{
    margin: 0;
    text-decoration: none;
    color: #535353;
    font-size: 0.9rem;
    font-weight: 600;  
    padding-left: 2px;
    padding-right: 20px;
    padding-top: 2px;
}
/*Desativando padding direito do texto carrinho*/
header .cabecalho .acesso div .t2{
    padding-right: 0;
}

/*Efeito passar mouse por cima do Menu*/
.grow:hover {
    transition-duration: 0.2s;
    -webkit-transform: scale(1.2);
    -ms-transform: scale(1.2);
    transform: scale(1.04);
}
/*-----------------------------------*/
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

@media (max-width: 1075px) {
    header .cabecalho nav .lista_form form input {
        width: 40vw;
    }
}

@media (max-width: 991px) {
    header .cabecalho nav .logo {
        display: none;
    }
    .grow:hover {
        transform: scale(1.0);
    }
    header .cabecalho nav .acesso {
        margin: 0;
    }
    header .cabecalho nav .lista_form ul li a {
        font-size: 0.9rem;
    }
    header .cabecalho nav .lista_form form input {
        width: 70vw;
    }
    header .cabecalho nav .lista_form {
        margin: 0;
    }

    header .cabecalho .logo2 {
        display: flex;
        width: 130px;
    }
}

@media (max-width: 790px) {
    header .cabecalho nav .lista_form form input {
        width: 60vw;
    }
    
}

@media (max-width: 500px) {
    header .cabecalho nav .acesso a img {
        width: 20px;
    }
    
    header .cabecalho nav .lista_form form input {
        width: 50vw;
    }
    header .cabecalho .logo2 {
        width: 100px;  
    }

    header .cabecalho .acesso div .text {
        display: none;
    }
    header .cabecalho .acesso div a {
        padding-left: 15px;
    }
}

</style>