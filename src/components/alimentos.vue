<template>
    <div class="corpo">
        <b-container fluid class="cont">
            <b-row>
                 <b-col lg="1"></b-col>
                <b-col cols="11" lg="4"  align-self="center">
                     <b-row >
                        <b-col cols="12" lg="5"><div class="obra"></div></b-col>
                    </b-row>
                    <b-row>
                        <b-col cols="12" >
                            <div class="acess">
                                Rapidez e praticidade para obter o
                                planejamento completo da obra, com
                                cronogramas físico-financeiro,
                                histograma de mão de obra e
                                equipamentos. Mais transparência,
                                economicidade e resultados.
                            </div>
                        </b-col>   
                    </b-row>
                </b-col>
                <b-col lg="1"></b-col>
                <b-col cols="12" lg="5">
                    <div class="engine"></div>
                </b-col>
                <b-col lg="1"></b-col>
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
     
        background: linear-gradient(-45deg,   #49626f, #7695a1 );
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
    line-height: 1.6;
    
    }
   
.engine{
    min-height: 400px;
    background: url('./img/alimento2.jpg');
    background-size: cover;
}
.obra{
    min-height: 130px;
    min-width: 35em;
    background: url('./img/alimento.png');
    background-size: contain;
    background-repeat: no-repeat;
    display: block;
}
.tes{
    background: url('./img/listaverde.png');
    background-size: cover;
    height:24vh;
    min-width: 95vw;
    z-index: 9999;
    position:absolute;
    margin-top: -10vh;
    margin-left: -8vw
}
.cont{
    margin:10vh 0vh;
}
.ko{
    display:block;
    align-content: center;
}
    @media only screen and (max-width: 991px){
        .tes{ display:none; }
        .engine{ display:none; }
}
</style>