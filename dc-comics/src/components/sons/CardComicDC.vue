<template>
  <div>
    <div class="cardDC">
        <img :src="thumb" :alt="type">
        <h3>{{series}}</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardComicDC',
  props:{
      thumb: String,
      series: String,
      type: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

img{
    object-fit: contain;
}

h3{
    text-align: start;
    padding: 0 70% 0 0;
}

</style>