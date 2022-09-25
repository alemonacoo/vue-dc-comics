<template>
<footer>
    <TopFooter/>
    <MiddleFooter/>
    <BottomFooter/>
</footer>
</template>

<script>
import TopFooter from './topFooter.vue';
import MiddleFooter from './middleFooter.vue';
import BottomFooter from './bottomFooter.vue';


export default {
    name: 'FooterComponent',
    components:{
         TopFooter,MiddleFooter, BottomFooter}

}
</script>

<style lang="scss" scoped>
@import '../main.scss';

</style>