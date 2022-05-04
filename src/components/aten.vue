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
                   
    <div>
               <b-row align-h="center" class="prefeituras">
                   <b-col cols="12" md="2" class="cba"></b-col>
                   <b-col cols="12" md="2" class="pxr"></b-col>
                   <b-col cols="12" md="2" class="tbc"></b-col>
                   <b-col cols="12" md="2" class="jcr"></b-col>
                   <b-col cols="12" md="2" class="alm"></b-col>
                   <b-col cols="12" md="2" class="cdg"></b-col>
               </b-row>
    </div>
    <div class="foote">
      <div>Tecnologia <strong>ABRANGE</strong> Resultados nems </div>
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
    display:flex;
    align-items: center;
    justify-content: center;
    background:linear-gradient(45deg,   #59727f, #86a5b1 );
    background-size: contain;
    height: 11vw;
    color:#f9f9f9;
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
    background: url('./img/not.png');
    height: 22rem;
    width: 38rem!important;
    background-size: cover;
    width: 50vw;
    border:0px;
 }
 .contedor {
     
     display:flex;
     justify-content: center;
     padding:1em;
 }
 .prep{padding-top: 11em;}
 .prefeituras{
        width:100vw;
 }
 .cba{background:url('./img/rosario.png'); height: 10rem; width:10rem;  background-size: cover; }
 .tbc{background:url('./img/nova.png'); height: 10rem; width:10rem;  background-size: cover; }
 .pxr{background:url('./img/diamantino.png'); height: 10rem; width:10rem;  background-size: cover; }
 .jcr{background:url('./img/amm.png'); height: 10rem; width:10rem;  background-size: cover; }
 .alm{background:url('./img/peixoto.png'); height: 10rem; width:10rem;  background-size: cover; }
 .cdg{background:url('./img/barra.png'); height: 10rem; width:10rem;  background-size: cover; }

     @media only screen and (max-width: 1400px){ 
.cba{background:url('./img/rosario.png'); height: 10rem; width:10rem;  background-size: cover;}
 .tbc{background:url('./img/nova.png'); height: 10rem; width:10rem;  background-size: cover;}
 .pxr{background:url('./img/diamantino.png'); height: 10rem; width:10rem;  background-size: cover;}
 .jcr{background:url('./img/amm.png'); height: 10rem; width:10rem;  background-size: cover;}
 .alm{background:url('./img/peixoto.png'); height: 10rem; width:10rem;  background-size: cover;}
 .cdg{background:url('./img/barra.png'); height: 10rem; width:10rem;  background-size: cover;}
 }
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
p{font-size: 10pt;}
 }
</style>