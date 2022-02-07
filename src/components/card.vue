<template>
    <div class="card">
        <div class="msg">
            <h1>Todo negócio, <strong class='laranja'>ABRANGE</strong><br>grandes projetos.</h1>
        </div>
    </div>
</template>




<script>
export default {

}
</script>

<style scoped>
h1{color:aliceblue; font-weight: 400;}
.card{
        height:62vh;
        display:flex;
        background: url('./img/topo.png');
        background-size: cover;
        align-items: center;
        font-family: 'Light';
    }
.msg{
    font-size: 9pt;
    margin-left: 11vw;
    text-align: left;
    transform: scaleY(1.13);
 }
 @media only screen and (max-width: 1000px){
   .texto{
     width: 30vw;
    font-size: 1.35em;
         }
}
</style>