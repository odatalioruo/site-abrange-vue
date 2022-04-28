<template>

    <div id="contato" class="imag">
        <div class="pen">
            <div class="card"></div>
        </div>
    </div>
    
    <b-row class="mt-5 " >
        <b-col cols="12" md="6" class="jasjaksjdlaskdjlsakjdlka">
            <b-row class="justify-content-center">
                <b-col cols="12" md="6"></b-col>
                <b-col cols="5" md="2"><div class="fotoum"></div></b-col>
                <b-col cols="5" md="4"><p><strong>Central de Atendimento<br>
                (65) xxxx xxxx</strong><br>
                Seg a sex - 8h às 11h30 de 13 às 17h30</p></b-col>
            </b-row>
            
            
        </b-col>
        <b-col cols="12" md="6" class="jasjaksjdlaskdjlsakjdlka">
            <b-row class="justify-content-center">
            <b-col cols="5" md="2"><div class="fotodois"></div>           
            </b-col>
            <b-col cols="5" md="4">
                <p><strong>E-mail</strong><br>
                Seg a sex - 8h às 11h30 de 13 às 17h30</p>
            </b-col>
            <b-col cols="12" md="6"></b-col>
            </b-row>
            
        </b-col>

    </b-row>
                   <h1 class="laranja mt-5 pt-5">PARCEIROS</h1>
    <div class="prefeituras">
 
                <div class="penis">
                    
                        <b-col cols="12" sm="12" v-for="(item,index) in prefi" :class="item.class" v-bind:key="index">
                            <div :class="item.class2"></div>
                        </b-col>
                    
                </div>
    </div>
    <div class="foote">
      <div></div>
    </div>


</template>


<script>
export default {
    name: 'Atend',
    data() {
        return {
        prefi: [
            {id: 1, class: "a", class2:"cba"},
            {id: 2, class: "b", class2:"pxr"},
            {id: 3, class: "c", class2:"tbc"},
            {id: 4, class: "d", class2:"jcr"},
            {id: 5, class: "e", class2:"alm"},
            {id: 6, class: "f", class2:"cdg"}
        ]
    }
    },
}
</script>

<style scoped>

.foote
{
    background: url('./img/rodape.png');
    background-size: cover;
    height: 25.4vw;
}
p { 
    color:#72849a;
    font-size: 11pt;
    text-align: left;
}

.fotoum {
        background:url('./img/icon_atendimento.png');
        background-size: 4.5em;
        background-repeat: no-repeat;
        min-height: 4.5em;
        min-width: 4.5em;
    }

.fotodois {
       background:url('./img/icon_email.png');
       background-size: 4.5em;
       background-repeat: no-repeat;
       min-height: 4.5em;
       min-width: 4.5em;
     }

.pen{
    padding-top: 80px;
    display:flex;
    justify-content: center;
}
.card {
    background: url('./img/NOT.png');
    height: 25rem;
    width: 35rem!important;
    background-size: cover;
    width: 50vw;
 }
 .contedor {
     
     display:flex;
     justify-content: center;
     padding:1em;
 }
 .prep{padding-top: 11em;}
.penis {  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr;
  grid-auto-columns: 1fr;
  grid-auto-rows: 1fr;
  gap: 0px 0px;
  grid-auto-flow: row;
  grid-template-areas:
    "a b c d e f";
    width:70vw;
}

 .prefeituras{
         justify-content: center;
         display: flex;
         margin:2em;
 }
 .cba{background:url('./img/rosario.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
 .tbc{background:url('./img/nova.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
 .pxr{background:url('./img/diamantino.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
 .jcr{background:url('./img/amm.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
 .alm{background:url('./img/peixoto.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
 .cdg{background:url('./img/barra.png'); height: 10em; background-size: cover; padding-bottom: 2em;}


 @media only screen and (max-width: 762px){
      #contato{
                display:none;
            }
            .jasjaksjdlaskdjlsakjdlka{
    display: flex;
    justify-content: center;
}
            .justify-content-center{
    display: flex;
    justify-content: center;
}
 }


</style>