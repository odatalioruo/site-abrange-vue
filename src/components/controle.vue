<template>
    <div class="corpo">
        <b-container fluid class="cont">
            
            <b-row align-v="center">
                <b-col sm="1"></b-col>
                <b-col sm="5" class="ko">
                
                <b-row>
                    <b-col sm="6"><div class="obra"></div>   </b-col> <b-col></b-col>
                </b-row>
                    
                    
                    <div class="acess">
                        Rapidez e praticidade para obter o
                        planejamento completo da obra, com
                        cronogramas físico-financeiro,
                        histograma de mão de obra e
                        equipamentos. Mais transparência,
                        economicidade e resultados.
                    </div>    
                </b-col>
                <b-col><div class="engine" align-self="stretch"></div> </b-col>
                <b-col sm="1">               
                </b-col>
            </b-row>
                <div class="tes"></div>
        </b-container>
       
        
    </div>
</template>


<script>
a
var a = `
            Rapidez e praticidade para obter o
            planejamento completo da obra, com
            cronogramas físico-financeiro,
            histograma de mão de obra e
            equipamentos. Mais transparência,
            economicidade e resultados.
        `
export default {
    
}
</script>
<style scoped>
h1{font-family: 'Bold'; margin-bottom: 1px; line-height: 1.1;}
p{margin-top: 11px;}
    .corpo{ 
     
        background: linear-gradient(-45deg,  #7695a1 , #49626f);
        background-size: cover;
        font-family: 'Light';
        color:whitesmoke;
        overflow: hidden;
        position:relative;
        z-index: 1;
    }
    .acess{
    padding: 2em 0;
    font-size: 1.3em;
    /* margin-left: 8vw; */
    text-align: left;
    width: 75%;
    line-height: 1.6;
    
    }
    @media only screen and (max-width: 1500px){
   .acess{
       width: 25vw;
       font-size: 1.2em;
         }
}
.engine{
    height: 50vh;
    background: url('./img/roxa.jpg');
    background-size: cover;
}
.obra{
    min-height: 7vw;
    width: 135%;
    background: url('./img/controle4.png');
    background-size: contain;
    background-repeat: no-repeat;
    display: block;
}
.tes{
    background: url('./img/listaroxa.png');
    background-size: cover;
    height:24vh;
    min-width: 85vw;
    z-index: 9999;
    position:absolute;
    margin-top: -12vh;
}
.cont{
    margin:10vh 0vh;
}
.ko{
    display:block;
    align-content: center;
}
</style>