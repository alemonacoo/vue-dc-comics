<template>
  <div id="app">
    <HeaderComponent/>
    <MainComponent :comics="comics"/>
    <FooterComponent/>

  </div>
</template>

<script>
import HeaderComponent from '@/components/header/HeaderComponent.vue'
import MainComponent from '@/components/main/MainComponent.vue'
import FooterComponent from '@/components/footer/FooterComponent.vue'
import comics from '@/assets/data/dc-comics.json'


export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
  },
  data(){
    return{comics}
  }
}
</script>

<style lang="scss">
*{
  font-family: 'Oswald', sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
