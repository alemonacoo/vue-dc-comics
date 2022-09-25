<template>
  <main>Content Goes Here !</main>
</template>

<script>
export default {
    name: 'MainComponent'

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