<template>
  <div>
    <div class="row">
       <div class="column">
           <ul>
               <li v-for="(element, index,) in menuFooterLinkTitles" :key="index">
                   <h3>{{element.title}}</h3>
                   <a  v-for="(element, index,) in element.links" :key="index" 
                   href="#">{{element.link}}</a>
                </li>
            </ul>
       </div>
       <div class="column container_img margin0">
       </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterUpper',
  data(){
      return{
          menuFooterLinkTitles: [
              {
                  title: 'dc comics',
                  links:[
                    {
                      link: 'Characters'
                    },
                    {
                      link: 'Comics'
                    },
                    {
                      link: 'Movies'
                    },
                    {
                      link: 'TV'
                    },
                    {
                      link: 'Games'
                    },
                    {
                      link: 'Videos'
                    },
                    {
                      link: 'News'
                    },
                  ]
              },
              {
                  title: 'shop',
                  links:[
                    {
                      link: 'Shop DC'
                    },
                    {
                      link: 'Shop DC Collectibles'
                    },
                  ]
              },

              {
                  title: 'dc',
                  links:[
                    {
                      link: 'Term Of Use'
                    },
                    {
                      link: 'Privacy Policy (New)'
                    },
                    {
                      link: 'Ad Choices'
                    },
                    {
                      link: 'Advertising'
                    },
                    {
                      link: 'Jobs'
                    },
                    {
                      link: 'Subscriptions'
                    },
                    {
                      link: 'Talent Workshops'
                    },
                    {
                      link: 'CPSC Certificates'
                    },
                    {
                      link: 'Ratings'
                    },
                    {
                      link: 'Shop Help'
                    },
                    {
                      link: 'Contact Us'
                    },
                  ]
              },
              {
                  title: 'site',
                  links:[
                    {
                      link: 'DC'
                    },
                    {
                      link: 'Mad Magazine'
                    },
                    {
                      link: 'DC Kids'
                    },
                    {
                      link: 'Dc Universe'
                    },
                    {
                      link: 'DC Power Visa'
                    },
                  ]
              },
          ],
      }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../style/pater.scss';

ul{
    list-style-type: none;
    display: flex;
    justify-content: space-between;
    padding: 60px 30px;

    li{
        display: flex;
        align-items: start;
        flex-direction: column;
        color: $txt-whi;
        margin: 10%;

        h3{
            color: $txt-whi;
            text-transform: uppercase;
            font-weight: bold;
          }

        a{
            display: flex;
            flex-direction: column;
            text-decoration: none;
            color: $txt-gr;
            margin: 2% 0;
            
         }
      }
  }

 .row{
     display: flex;
     flex-direction: row;
     justify-content: start;
     width: 80%;
     height: 100%;
 }

  .column{
     display: flex;
     flex-direction: row;
     justify-content: center;
     width: 50%;
     height: auto;
 }

 .container_img{
     display: flex;
     width: 30%;
     height: auto;
     background-image: url('../assets/img/dc-logo-bg.png');
     background-repeat: no-repeat;
     background-size: cover;
     background-position-y: 50%;
 }
.margin0{
    margin-left: 20%;
}

.flexcol{
    flex-direction: column;
}
    
</style>