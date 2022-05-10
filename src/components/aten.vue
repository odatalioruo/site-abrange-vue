<template>

    <div id="contato" class="imag">
        <div class="pen">
            <div class="card"></div>
        </div>
    </div>
<div class="screen">
    <b-row class="mt-5">
        <b-col cols="12" md="6" class="jasjaksjdlaskdjlsakjdlka">
            <b-row class="justify-content-center">
                <b-col cols="2" lg="6"></b-col>
                <b-col cols="3" lg="1"><div class="fotoum"></div></b-col>
                <b-col cols="7" lg="5"><p><strong>Central de Atendimento<br>
                (65) xxxx xxxx</strong><br>
                Seg a sex - 8h às 11h30 de 13 às 17h30</p></b-col>
            </b-row>
            
            
        </b-col>
        <b-col cols="12" md="6" class="jasjaksjdlaskdjlsakjdlka">
            <b-row class="justify-content-center">
            <b-col cols="5" md="1"><div class="fotodois"></div>           
            </b-col>
            <b-col cols="5" md="5">
                <p><strong>E-mail</strong><br>
                Seg a sex - 8h às 11h30 de 13 às 17h30</p>
            </b-col>
            <b-col cols="12" md="6"></b-col>
            </b-row>
            
        </b-col>

    </b-row>
</div>
<div class="smallsc">
        <b-row class="mt-5">
            <b-col cols="12" md="6" class="jasjaksjdlaskdjlsakjdlka">
                <b-row class="justify-content-center">
                    <b-col cols="2"></b-col>
                    <b-col cols="3"><div class="fotoum"></div></b-col>
                    <b-col cols="7"><p><strong>Central de Atendimento<br>
                    (65) xxxx xxxx</strong><br>
                    Seg a sex - 8h às 11h30 de 13 às 17h30</p></b-col>
                </b-row>
                
                
            </b-col>
            <b-col cols="12" md="6" class="jasjaksjdlaskdjlsakjdlka">
                <b-row class="justify-content-center">
                     <b-col cols="2" ></b-col>
                <b-col cols="3"><div class="fotodois"></div>           
                </b-col>
                <b-col cols="7">
                    <p><strong>E-mail</strong><br>
                    Seg a sex - 8h às 11h30 de 13 às 17h30</p>
                </b-col>
                
                </b-row>
                
            </b-col>

    </b-row>
</div>
                   <h1 id="parceiros" class="laranja mt-5 pt-5">PARCEIROS</h1>
                   
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
<div class="asd">
    <b-row class="foote">
        <b-col cols="12" md="3" class="a"></b-col>
        <b-col cols="12" class="emago"></b-col>
        <b-col cols="12"></b-col>
 
    </b-row>

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
        ],
    }
    },
}
</script>

<style scoped>

.screen{
    display:contents;
}
.smallsc{
    display:none;
}
.foote
{
    display:flex;
    align-items: center;
    justify-content: center;
    background:linear-gradient(45deg,   #135, #9ab );
    background-size: cover;
    height: 24vh;
    color:#f9f9f9;
    flex-direction: column;
    overflow:hidden;

}
p { 
    color:#72849a;
    font-size: .8em;
    text-align: left;
}

.fotoum {
        background:url('./img/icon_atendimento.png');
        background-size: 3.5em;
        background-repeat: no-repeat;
        min-height: 3.5em;
        min-width: 3.5em;
    }

.fotodois {
       background:url('./img/icon_email.png');
       background-size: 3.5em;
       background-repeat: no-repeat;
       min-height: 3.5em;
       min-width: 3.5em;
     }

.pen{
    padding-top: 80px;
    display:flex;
    justify-content: center;
}
.card {
    background: url('./img/not.png');
    height: 200px;
    width: 22rem!important;
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
        margin-top:4em;
        margin-bottom:4em;
 }
 .cba{background:url('./img/rosario.png'); height: 10rem; width:10rem;  background-size: cover; }
 .tbc{background:url('./img/nova.png'); height: 10rem; width:10rem;  background-size: cover; }
 .pxr{background:url('./img/diamantino.png'); height: 10rem; width:10rem;  background-size: cover; }
 .jcr{background:url('./img/amm.png'); height: 10rem; width:10rem;  background-size: cover; }
 .alm{background:url('./img/peixoto.png'); height: 10rem; width:10rem;  background-size: cover; }
 .cdg{background:url('./img/barra.png'); height: 10rem; width:10rem;  background-size: cover; }

     @media only screen and (max-width: 1400px){ 
         .foote { height: 10em;}
.cba{background:url('./img/rosario.png'); height: 10rem; width:10rem;  background-size: cover;}
 .tbc{background:url('./img/nova.png'); height: 10rem; width:10rem;  background-size: cover;}
 .pxr{background:url('./img/diamantino.png'); height: 10rem; width:10rem;  background-size: cover;}
 .jcr{background:url('./img/amm.png'); height: 10rem; width:10rem;  background-size: cover;}
 .alm{background:url('./img/peixoto.png'); height: 10rem; width:10rem;  background-size: cover;}
 .cdg{background:url('./img/barra.png'); height: 10rem; width:10rem;  background-size: cover;}
 }
  .emago{
     background: url("./img/marca.png");
     background-size: cover;
     height: 42px;
     width: 210px;

 }
 @media only screen and (max-width: 900px){
      #contato{
                display:none;
            }
            .emago{  background: url("./img/marca.png");
                    background-size: cover;
                    width:16em;
                    height:3em;
            }
            .jasjaksjdlaskdjlsakjdlka{
    display: flex;
    justify-content: center;
}
.screen{
    display:none;
}
.smallsc{
    display:contents;
}
.justify-content-center{
    display: flex;
    justify-content: center;
}
 }
 .asd{background: #72849a;}
 .a{
     background:url('./img/A.png');
     background-size: cover;
     position:absolute;
     height: 38vh;
     width: 38vw;
     margin-left:58vw;
     overflow: hidden;
     margin-bottom: 14vh;
     max-width: 100vw;
}
</style> 