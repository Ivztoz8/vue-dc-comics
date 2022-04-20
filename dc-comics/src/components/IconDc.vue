<template>
  <div>
    <!-- Icon Menu -->
    <ul class="container">
        <li v-for="(element, index) in menuIcoLink" :key="index">
            <a :href="element.url"><img :src="element.img" :alt="element.alt" :class="element.class"></a>
            <h3><a :href="element.url">{{element.link}}</a></h3>
        </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'IconDc',
  data(){
      return{
          menuIcoLink: [
            {
              img: require('../assets/img/buy-comics-digital-comics.png'),
              alt: 'buy comics',
              link: 'digital comics',
              url: '#',
              class: 'size'
            },
            {
              img: require('../assets/img/buy-comics-merchandise.png'),
              alt: 'comics merchandise',
              link: 'dc merchandise',
              url: '#',
              class: 'size'
            },
            {
              img: require('../assets/img/buy-comics-subscriptions.png'),
              alt: 'subscription',
              link: 'subscription',
              url: '#',
              class: 'size'
            },
            {
              img: require('../assets/img/buy-comics-shop-locator.png'),
              alt: 'shop locator',
              link: 'comic shop locator',
              url: '#',
              class: 'size'
            },
            {
              img: require('../assets/img/buy-dc-power-visa.svg'),
              alt: 'power visa',
              link: 'dc power visa',
              url: '#',
              class: 'size2' 
            },
          ]
        }
      }
  }
</script>

<style scoped lang="scss">

@import '../style/vars.scss';

ul{
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    padding: 60px 30px;

    li{
        display: flex;
        align-items: center;
        color: $txt-whi;

        h3{
          margin-left: 20px;

           a{
            text-decoration: none;
            color: $txt-whi;
            text-transform: uppercase;
            font-weight: bold;
            }
          }
      }
  }

  .size{
    height: 70px;
  }
  .size2{
    height: 50px;
  }

</style>
