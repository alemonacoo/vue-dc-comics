<template>
<footer>
    <TopFooter/>
    <MiddleFooter/>
    <BottomFooter/>
</footer>
</template>

<script>
import TopFooter from '@/components/footer/topFooter.vue';
import MiddleFooter from '@/components/footer/middleFooter.vue';
import BottomFooter from '@/components/footer/bottomFooter.vue';


export default {
    name: 'FooterComponent',
    components:{
         TopFooter,MiddleFooter, BottomFooter}

}
</script>

<style lang="scss" scoped>
@import '@/components/main.scss';

</style>