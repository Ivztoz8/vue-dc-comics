<template>
  <div>
      <!-- Menu -->
      <ul>
          <li v-for="(element, index) in menuLink" :key="index">
             <a :href="element.url">{{element.link}}</a> 
          </li>
      </ul>
  </div>
    
</template>

<script>
export default {
  name: 'MenuTopDc',
  data(){
      return{
          menuLink: [
              {
                  link: 'characters',
                  url: '#'
              },
               {
                  link: 'comics',
                  url: '#'
              },
               {
                  link: 'movies',
                  url: '#'
              },
              {
                  link: 'tv',
                  url: '#'
              },
              {
                  link: 'games',
                  url: '#'
              },
              {
                  link: 'collectibles',
                  url: '#'
              },
              {
                  link: 'videos',
                  url: '#'
              },
              {
                  link: 'fans',
                  url: '#'
              },
              {
                  link: 'news',
                  url: '#'
              },
              {
                  link: 'shop',
                  url: '#'
              },
              

          ]
      }
  }
}
</script>


<style scoped lang="scss">

@import '../style/pater.scss';

ul{
    list-style-type: none;
    display: flex;
     :hover{
        border-bottom: 1px solid $txt-blue;
    }
    li{
        margin: 0 30px;
        
        a{
            text-decoration: none;
            text-transform: uppercase;
            color: $txt-grdrk;
            font-weight: bold;
        }
    }
}


</style>
