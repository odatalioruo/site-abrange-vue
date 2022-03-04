<template>
<div>
    <div id="contato" class="imag">
        <div class="pen">
            <div class="card"></div>
        </div>
    </div>
    
    <div class="contedor">
        <div class="container">
            <div class="fotoum">

            </div>
            <div class="Atendimento">
                 <p><strong>Central de Atendimento<br>
                (65) xxxx xxxx</strong><br>
                Seg a sex - 8h às 11h30 de 13 às 17h30</p>
            </div>
            <div class="fotodois">

            </div>
            <div class="email">
                <p><strong>E-mail</strong><br>
                Seg a sex - 8h às 11h30 de 13 às 17h30</p>
            </div>
        </div>
    </div>
        <div class="prep"></div>
                   <h1 class="laranja">PARCEIROS</h1>
    <div class="prefeituras">
 
                <div class="penis">
                    <div v-for="(item,index) in prefi" :class="item.class" v-bind:key="index">
                        <div :class="item.class2"></div>
                    </div>
                </div>
    </div>
    <div class="foote">
      <div></div>
    </div>
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
.container {  display: grid;
margin-left: 8em;
  grid-template-columns: 1fr 3.5fr 1fr 3.5fr;
  grid-template-rows: 1fr;
  grid-auto-columns: 1fr;
  grid-auto-rows: 1fr;
  gap: 0px 0px;
  grid-auto-flow: row;
  grid-template-areas:
    "fotoum Atendimento fotodois email";

    width: 55vw;
    color:#72849a;
    font-size: 11pt;
    text-align: left;
}

.fotoum {
     grid-area: fotoum;
      background:url('./img/icon_atendimento.png');
      background-size: 4em;
       background-repeat: no-repeat;
    }

.Atendimento { grid-area: Atendimento; }

.fotodois {
     grid-area: fotodois;
       background:url('./img/icon_email.png');
       background-size: 4em;
       background-repeat: no-repeat;
     }

.email { grid-area: email; }


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

.a { grid-area: a; }

.b { grid-area: b; }

.c { grid-area: c; }

.d { grid-area: d; }

.e { grid-area: e; }

.f { grid-area: f; }

 .prefeituras{
         justify-content: center;
         display: flex;
         
 }
 .cba{background:url('./img/rosario.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
 .tbc{background:url('./img/nova.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
 .pxr{background:url('./img/diamantino.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
 .jcr{background:url('./img/amm.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
 .alm{background:url('./img/peixoto.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
 .cdg{background:url('./img/barra.png'); height: 10em; background-size: cover; padding-bottom: 2em;}
</style>