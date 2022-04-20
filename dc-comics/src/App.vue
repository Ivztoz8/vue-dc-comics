<template>
  <div>
   <header class="mycontainer">
      <LogoDc/>
      <MenuTopDc/>
   </header>
   <main>
     <div class="jumbotron">
     </div>
     <div class="content">
       <div class="mycontainer relative">
         <div class="label-comic">
           current series
         </div>
          <ComicsDC/>
       </div>
     </div>
     <div class="icons">
       <IconDc/>
     </div>
   </main>
   <footer class="bg-img">
     <FooterUpper/>
     <FooterDowner/>
   </footer>
  </div>
</template>

<script>
import LogoDc from './components/LogoDc.vue'
import MenuTopDc from './components/MenuTopDc.vue'
import IconDc from './components/IconDc.vue'
import FooterUpper from './components/FooterUpper.vue'
import FooterDowner from './components/FooterDowner.vue'
import "bootstrap"
import ComicsDC from './components/ComicsDC.vue'


export default {
  name: 'App',
  components: {
    LogoDc,
    MenuTopDc,
    IconDc,
    FooterUpper,
    FooterDowner,
    ComicsDC
  }
}
</script>

<style lang="scss">

@import "bootstrap/dist/css/bootstrap.min.css";
@import './style/pater.scss';


header{

  @include flexBetwee(space-between, center);
  //justify-content: space-between;
  //align-items: center;
}

.content{
  background-color: $bg-black;
  color: $txt-whi;
  padding: 30px;
}

.icons{
  background-color: $bg-blue;
}

.bg-img{
    background-image: url('./assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}

.jumbotron{
  background-image: url('./assets/img/jumbotron.jpg');
  background-position: top;
  background-repeat: no-repeat;
  width: 100%;
  height: 50vh;
  background-size: cover;
}

.label-comic{
  display: inline-block;
  background-color: $bg-blue;
  padding: 20px 10px;
  position: absolute;
  top: -50px;
  left: 0;
}

</style>
