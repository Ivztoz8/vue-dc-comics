<template>
  <div>
   <header class="container">
       <LogoDc/>
      <MenuTopDc/>
   </header>
   <main>
     <div class="content">
       <div class="container">
         <h3>&#8594; Content Goes Here &#8592;</h3>
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


export default {
  name: 'App',
  components: {
    LogoDc,
    MenuTopDc,
    IconDc,
    FooterUpper,
    FooterDowner
  }
}
</script>

<style lang="scss">

@import './style/reset.scss';
@import './style/mixin.scss';
@import './style/global.scss';
@import './style/vars.scss';


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
</style>
