<template>
  <main>
    <div class="wallpaper"></div>
    <div class="comics-container"></div>
  </main>
</template>

<script>

export default {
    name: 'MainComponent',
    props:{
      comics: Array
    },  
    mounted() {
    console.log(this.comics);
  },

}
</script>

<style lang="scss" scoped>
@import '@/components/main.scss';
main{
  @include my-width;
  @include flex-row;
  align-items: center;
  min-height: 15vh;
  color: white;
  background-color: black;
}


</style>