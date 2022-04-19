<template>
  <div>
   <header class="container">
     <LogoDc/>
     <MenuTopDc/>
   </header>
   <main>
     <div class="content">
       <div class="container">
         <h3>Il contenuto va qui</h3>
       </div>
       
     </div>
     <div class="icons">
       <IconDc/>
     </div>
   </main>
  </div>
</template>

<script>
import LogoDc from './components/LogoDc.vue'
import MenuTopDc from './components/MenuTopDc.vue'
import IconDc from './components/IconDc.vue'


export default {
  name: 'App',
  components: {
    LogoDc,
    MenuTopDc,
    IconDc
  }
}
</script>

<style lang="scss">

@import './style/reset.scss';
@import './style/mixin.scss';
@import './style/global.scss';


header{

  @include flexBetwee(space-between, center);
  //justify-content: space-between;
  //align-items: center;
}

.content{
  background-color: black;
  color: white;
  padding: 30px;
}

</style>
