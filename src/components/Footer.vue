<template>
    <footer>
             <div class="footer">
                <span>
                    <strong>PETABYTE</strong> ATACADO E VAREJO DE PRODUTOS DE INFORMATICA LTDA <br>
                    <strong>ATEDIMENTO</strong><span></span> De segunda à sexta das 8h30 as 12h - 13h às 18H<br>
                    <strong>Campo Grande | MS</strong><br>
                    Siga-nos<br>
                </span>
                <a href="https://pt-br.facebook.com/"><i class="fa fa-facebook"></i></a>
                <a href="https://twitter.com/login?lang=pt"><i class="fa fa-instagram"></i></a>
                <a href="https://www.instagram.com/?hl=pt-br"><i class="fa fa-twitter"></i></a>
            </div>
        </footer>
</template>

<script>
export default {
    
}
</script>

<style>
footer {
    position: absolute;
    background-color:#161616;
    width: 100%;
    clear: both;
    padding: 20px 0;
    border-top: rgb(0, 140, 255) solid 4px;
    text-align: center;
    font-size: 0.8rem;
    
}
/*div do rodapé*/
footer .footer {
    width: 90%;
    max-width: 1200px;
    align-items: center;
    justify-content: space-between;
    margin: auto;
}
/*Cor do texto*/
footer .footer span {
    color: rgb(206, 206, 206);
}
/*Icones*/
footer div a {
    color: #868686;
    font-size: 1.3rem;
    padding: 10px; 
    transition: all .5s ease;
}

</style>