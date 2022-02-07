<template>
    <div class="corpo">
        <div class="acess">
        <h1>ACESSO<br>on-line</h1>
        <p>
            Rapidez e praticidade para obter o
            planejamento completo da obra, com
            cronogramas físico-financeiro,
            histograma de mão de obra e
            equipamentos. Mais transparência,
            economicidade e resultados.
        </p>
        </div>
    </div>
</template>


<script>
export default {
    
}
</script>
<style scoped>
h1{font-family: 'Bold'; margin-bottom: 1px; line-height: 1.1;}
p{margin-top: 11px;}
    .corpo{
     
        height:75vh;
        display:flex;
        background: url('./img/banner1.png');
        background-size: cover;
        align-items: center;
        font-family: 'Light';
        color:whitesmoke;
    }
    .acess{
    width: 24vw;
    font-size: 1.5em;
    /* margin-left: 8vw; */
    text-align: left;
    line-height: 1.4;
    padding: 7em;
    }
    @media only screen and (max-width: 1500px){
   .acess{
       width: 25vw;
       font-size: 1.2em;
         }
}
</style>