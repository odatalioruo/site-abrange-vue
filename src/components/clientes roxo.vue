<template>
   
    <div class="corpo">
        <b-row class="center">
            <b-col cols="12" lg="3">
                   <div class="cont">
                    <div class="imagem" @mousedown.middle="redirect"></div>
                    </div>
            </b-col>
            <b-col cols="12" lg="4">
                <div class="texto">
             <h1 class="roxo">App exclusivo para clientes</h1>
            <p>
                compra inovadora, o processo de pagamento e
                finalização de compras é mais fácil, rápido e
                seguro. fácil navegação oferece, ainda, acesso
                ao endereço de todas as lojas cadastradas.
                O aplicativo, que está disponível para os
                sistemas Android e iOS. 
            </p>
        </div>
            </b-col>
        </b-row>
    </div>
</template>




<script>
export default {
    methods:{
         redirect: function (){
            window.location='https://www.youtube.com/watch?v=cnXYG0Om1dc'

        }
    }
}
</script>

<style scoped>
h1{line-height: 1.1; font-size:2.5em;}
.corpo{
    text-align: left;
    display: flex;
    justify-content: center;
    align-items: center;
    margin:5em 0em;
    font-family: 'Regular';
    height: 600px;
    overflow: hidden;
}

.roxo{
       color:rgb(140,70,207); 
   font-family: 'Bold'!important;
}
.texto {
     font-size: 1.1em;
     color: #575c66;
     line-height: 1.4;
     transform:scaleY(1.16);
     
     }


.imagem {
    background:url('./img/controle3d.png');
    background-size: contain;
    background-repeat: no-repeat;
    grid-area: imagem;
    width: 200px; 
    height: 200px;
     }

    .cont{
        display: flex;
        justify-content: right;
    }

 @media only screen and (max-width: 800px){
   .texto{
    margin:2em;
    font-size: 1.35em;
    padding:2em;
         }
 
} 


@media only screen and (max-width: 512px){
       .imagem{
    width:190px; 
    height:190px;
    }
}

@media only screen and (max-width: 1020px){
    .texto{font-size: 0.9em; margin:2em;}

    .cont{
         justify-content: center;
    }
}
</style>