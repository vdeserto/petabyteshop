<template>

    <Header/>

    <section>
        <div id="loginPage" class="container mb-4 mt-4">
        <!-- Inicio do container -->

            <!-- Tela de Login -->     
            <div id="login">
                <form>
                    <div class="col-10 ml-3 mt-3">
                        <h2 class="title">Fazer Login</h2>
                        <div class="form-group">
                            <input type="email" class="form-control" id="emailLogin" aria-describedby="emailHelp" placeholder="Email">
                        </div>

                        <div class="form-group submit">                            
                            <input type="password" class="form-control" id="senhaLogin" placeholder="Senha">
                                <span toggle="senhaLogin">
                                    <img src="../images/icons/eye.svg" id="eye" onclick="mostraSenha('senhaLogin', 'eye')">
                                </span>                                                           
                        </div>

                        <div class="submit">
                            <button type="submit" class="btn btn-primary">Fazer Login</button>
                            <a href="./forgot-password.html"><strong>Esqueceu a senha?</strong></a>
                        </div>
                    </div>
                </form>
            </div>      
            <!-- Tela de Cadastro -->       
            <div id="cadastro">
                <form>
                    <div class="col-10 ml-3 mt-3">
                        <h2 class="title">Criar uma conta</h2>
                        <div class="form-group">
                            <input type="text" class="form-control" id="nomeCadastro" placeholder="Nome">
                        </div>
                        <div class="form-group">
                            <input type="text" class="form-control" id="sobrenomeCadastro" placeholder="Sobrenome">
                        </div>
                        <div class="form-group">
                            <input type="email" class="form-control" id="emailCadastro" placeholder="Email">
                        </div>
                        <div class="form-group submit" >                            
                            <input type="password" class="form-control" id="senhaCadastro" placeholder="Senha">
                            <span toggle="#senhaCadastro">
                                <img src="../images/icons/eye.svg" id="eyeCadastro" onclick="mostraSenha('senhaCadastro','eyeCadastro')">
                            </span>                                
                        </div>
                        <div class="form-group">
                            <small class="row">A senha deve conter pelo menos 8 caracteres.</small>
                        </div>
                        <div class="form-group">
                            <small class="row">Um e-mail será enviado para verificação do seu endereço de e-mail. 
                                Clique no link do e-mail recebido para concluir a verificação.</small>
                        </div>
                        <div class="submit">
                            <button type="submit" class="btn btn-primary">Criar Conta</button>
                        </div>    
                    </div>
                </form>
            </div>
            <!-- Final do container -->
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
  name: "Login",

  components:{
      Header, 
      Footer
  }
  
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:ital,wght@0,300;0,400;0,600;0,700;1,300;1,400&display=swap');
/* O corpo da página de Login */
#loginPage {    
    border: 2px solid #0000005b;
    margin-bottom: 30%; 
    padding-left: 0%;   
    padding-right: 0%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    width: 80vw;
    max-width: 980px;
    max-height: 725px;   
}

.title {
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-size: 28px;
}

#login {
    width: 70%;
    padding: 2.5%;
    min-width: 50%;
} 

 /* Login spacement */
div.form-group {
    margin-top: 10%;
}

/* Login Password Input */
#senhaLogin, #senhaCadastro{
    box-sizing: border-box;
    display: flex;
    padding-right: 5%;
}

/* Password Field */
#passwordField {
    justify-content: center;
    display: flex;
    flex-direction: row;
}

/* Show Password */
#eye, #eyeCadastro {
    transform: translate(-125%,-50%);
    position: absolute;
    cursor: pointer;
    width: 7.5%;
    height: 100%;
    z-index: 1;
}

/* Div that contains Login and Submit */
.submit {
    justify-content: space-around;
    display: flex;
    flex-direction: row;
    align-items: center;

}

/* Login Forgot Password */
#login a {
    text-decoration: none;
    color: rgb(0, 78, 245);   
}

/* Login Forgot Password (Hover State) */
#login a:hover {
    color: (0px 0px 2px rgb(0, 81, 255));
    filter: drop-shadow(0px 0px 2px rgb(187, 208, 255));
}

/* SignIn display form */
#cadastro {
    background-color:#0000002e;
    display: flex;
    margin-right: 0%;
    padding: 2.5%;
    
    
}
/* SignIn div */

/* SignIn Password */
#senhaCadastro {
    box-sizing: border-box;
    display: flex;
}
/* SignIn small text */
#cadastro small {
    margin-left: 1.5%;
    margin-right: 1.5%;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}

/* SignIn Btn */
#cadastro button {
    margin-top: 5%;
}

/*Responsivo da página login*/
@media (max-width: 1075px) {

    .title {
        font-size: 1.5em ;        
    }
    
    #login {
        width: 70%;
        padding: 2.5%;
    } 

    #cadastro{
        width: 70%;
        padding: 2.5%;
    }

    .submit button {
        width: 35%;
        height: 20%;
        font-size: 0.8em;
        padding: 0.4em;
    }

    .submit a {
        font-size: 0.95em;
    }

    /* SignIn small text */
     #cadastro small {
        font-size: 0.725em;
    } 

    
}

@media (max-width: 991px) {
    div.col-10.ml-3.mt-3{
        padding: 0px!important;
    }

    .title {
        font-size: 1.5em ;        
    }
    
    #login {
        width: 70%;
        padding: 2.5%;
    } 

    #cadastro{
        width: 70%;
        padding: 2.5%;
    }

    .submit button {
        width: 45%;
        height: 30%;
        font-size: 0.7em;
        padding: 0.4em;
    }

    .submit a {
        font-size: 0.75em;
    }

    /* SignIn small text */
     #cadastro small {
        font-size: 0.6725em;
        line-height: 1.5em;
        
    } 
}

@media (max-width: 790px) {
    div.col-10.ml-3.mt-3{
        padding: 0px!important;
    }
    
    input.form-control{
        height: 30px;
        font-size: 0.75em;
    }

    .title {
        font-size: 1em ;        
    }
    
    #login {
        width: 50%;
        padding: 2.5%;
    } 

    #cadastro{
        width: 70%;
        padding: 2.5%;
    }

    .submit button {
        width: 80px;
        height: 25px;
        font-size: 0.6em;
        padding: 0.2em;
    }

    .submit a {
        font-size: 0.5em;
        
    }    
}

@media (max-width: 500px) {
    div.col-10.ml-3.mt-3{
        padding: 0px!important;
        margin: 0;
    }
    input.form-control{
        height: 5vh;
        font-size: 0.75em;
    }

    .title {
        font-size: 0.899em ;        
    }
    
    #login {
        width: 70%;
        padding: 2.5%;
    } 
    #login form {
        margin-top: 10px;
    }

    #cadastro{
        width: 70%;
        padding: 2.5%;
    }

    .submit {
        flex-direction: column-reverse;        
    } 

    #eye, #eyeCadastro {
        width: 4vw;
        height: 8vh;
        transform: translate(625%,-20%);
    }

    .submit a {
        font-size: 70%;
        margin-bottom: 10%;
        
    }   
    #loginPage{
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 150vh;
    }

    #login{
        height: 80vh;
        margin: auto;
        width: 100%;
    }
    #cadastro{
        width: 100%;
        height: 100%;
    }
    #cadastro button {
        margin: 0;
    }
}
@media (max-width: 320px) {
    #loginPage{
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 150vh;
    }

    #login{
        margin-bottom: 10vh;
        width: 100%;
        height: 30%;
    }
    #cadastro{
        width: 100%;
        height: 70%;
    }

}
</style>