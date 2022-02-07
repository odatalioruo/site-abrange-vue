<template>
   
    <div class="corpo">
        <div class="container">
        <div class="texto">
             <h1 class="laranja">App exclusivo<br> para clientes</h1>
            <p>
                compra inovadora, o processo de pagamento e
                finalização de compras é mais fácil, rápido e
                seguro. fácil navegação oferece, ainda, acesso
                ao endereço de todas as lojas cadastradas.
                O aplicativo, que está disponível para os
                sistemas Android e iOS. 
            </p>
        </div>
        <div class="imagem" @mousedown.middle="redirect"></div>
        </div>
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
    margin:5em 5em;
    font-family: 'Regular';
    height: 600px;
    overflow: hidden;
}

.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr;
  gap: 0px 0px;
  grid-auto-flow: row;
  grid-template-areas:
    "texto imagem"
    ;
}

.texto {
     grid-area: texto; 
     width: 34vw;
     font-size: 1.15em;
     color: #575c66;
     line-height: 1.4;
     transform:scaleY(1.13);
     }


.imagem {
    margin-left:5vw;
    background:url('./img/APP.png');
    background-size: contain;
    background-repeat: no-repeat;
    grid-area: imagem; 
    min-height: 350px;
     }

/* @media only screen and (max-width: 1500px){
   .texto{
     width: 25vw;
    font-size: 1.35em;
         }
} */
 @media only screen and (min-width: 1800px){
   .texto{
     width: 30vw;
    font-size: 1.35em;
  
         }
}
@media only screen and (max-width: 1020px){
    .texto{font-size: 0.9em;}
}
</style>