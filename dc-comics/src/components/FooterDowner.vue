<template>
  <div class="bg_darkgray padding0">
    <div class="row container">
      <div class="container">
      <div class="bg_darkgra"><a class="button padding1" href="#">SING-UP NOW!</a></div>
    </div>
    <div class="column">
      <ul>
        <li><h3>FOLLOW US</h3></li>
        <li v-for="(element, index) in IconsLinkList" :key="index">
         <a href="#"><img :src="element.img" :alt="element.alt"></a> 
        </li>
      </ul>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterDowner',
  data(){
    return{
      IconsLinkList: [
        {
          img: require('../assets/img/footer-facebook.png'),
          alt: 'facebook'
        },
        {
          img: require('../assets/img/footer-twitter.png'),
          alt: 'twitter'
        },
        {
          img: require('../assets/img/footer-youtube.png'),
          alt: 'youtube'
        },
        {
          img: require('../assets/img/footer-pinterest.png'),
          alt: 'pinterest'
        },
        {
          img: require('../assets/img/footer-periscope.png'),
          alt: 'periscope'
        },
      ]
    }
  }
}
</script>

<style scoped lang="scss">

@import '../style/global.scss';
@import '../style/vars.scss';

.bg_darkgray{
  background-color: $bg-grdrkhg;
}

.button{
  border: 1px solid $bg-blue;
}

.padding0{
  padding: 3%;
}

.padding1{
  padding: 1%;
}

a{
  text-decoration: none;
  color: $txt-whi;           
}

.row{
  display: flex;
  width: 80%;
  flex-direction: row;
  justify-content: start;
  align-items: center;
}

.column{
  display: flex;
  width: 50%;
  align-items: center;
  flex-direction: column;
}

ul{
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    padding: 60px 30px;

    li{
        display: flex;
        align-items: center;
        color: $txt-blue;

        h3{
            color: $txt-blue;
            text-transform: uppercase;
            font-weight: bold;
          }

        a{
            display: flex;
            text-decoration: none;
            color: $txt-gr;
            padding-left: 20px;
            margin: 2% 0;

         }
      }
  }

</style>