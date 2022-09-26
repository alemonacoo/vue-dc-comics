<template>
  <main>
    <div class="wallpaper">
    </div>
    <div class="comics-container">
      <div v-for="card in comics" :key="card.series">
      <CardComponent :card="card"/>
      </div>
    </div>
  </main>
</template>

<script>
import CardComponent from '@/components/main/cardComponent.vue';

export default {
    name: 'MainComponent',
    components:{
      CardComponent
    },
    props:{
      comics: Array
    },  
    mounted() {
    console.log(this.comics, 'ricevuto da main component');
  },

}
</script>

<style lang="scss" scoped>
@import '@/components/main.scss';
main{
  align-items: center;
  min-height: 15vh;
  color: white;
  width: 100vw;
  .wallpaper{
    color: white;
    height: 23vw;
    background-image: url(@/assets/img/jumbotron.jpg);
    background-size: cover;
  }
  .comics-container{
    @include my-width;
    @include flex-row;
    flex-wrap: wrap;
    min-height: 50vh;
    background-color: rgb(28,28,28);
  }
    



}


</style>