<template>
    <!--    <div class="carde">
                <div class="mesg">
                    <h1>Todo negócio, <strong class='laranja'>ABRANGE</strong><br>grandes projetos.</h1>
                </div>
            </div> -->
 
    <!--  -->
   <div class="pic-ctn">
       <div class="carde pic">
                <div class="mesg">
                    <h1>Todo negócio, <strong class='laranja'>ABRANGE</strong><br>grandes projetos.</h1>
                </div>
        </div>
    <img src="https://picsum.photos/200/300?t=1" alt="" class="pic">
    <img src="https://picsum.photos/200/300?t=2" alt="" class="pic">
    <img src="https://picsum.photos/200/300?t=3" alt="" class="pic">
    <img src="https://picsum.photos/200/300?t=4" alt="" class="pic">

  </div>
    <!--  -->
</template>




<script>
export default {

}
</script>

<style scoped>
h1{color:aliceblue; font-weight: 400;}
.carde{
        height:62vh;
        display:flex;
        background: url('./img/topo.png');
        background-size: cover;
        align-items: center;
        font-family: 'Light';
    }
.mesg{
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
/*  */


html, body {
  margin: 0;
  padding: 0;
}

.pic-ctn {
  width: 100vw;
  height: 200px;
}

@keyframes display {
  0% {
    transform: translateX(200px);
    opacity: 1;
  }
  10% {
    transform: translateX(0);
    opacity: 1;
  }
  20% {
    transform: translateX(0);
    opacity: 1;
  }
  30% {
    transform: translateX(-200px);
    opacity: 0;
  }
  100% {
    transform: translateX(-200px);
    opacity: 0;
  }
}

.pic-ctn {
  position: relative;
  width: 100vw;
  height: 300px;
  margin-top: 15vh;
}

.pic-ctn > img {
  position: absolute;
  top: 0;
  left: calc(50% - 100px);
  opacity: 0;
  animation: display 10s infinite;
}

img:nth-child(2) {
  animation-delay: 2s;
}
img:nth-child(3) {
  animation-delay: 4s;
}
img:nth-child(4) {
  animation-delay: 6s;
}
img:nth-child(5) {
  animation-delay: 8s;
}
</style>