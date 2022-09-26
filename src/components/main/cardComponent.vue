<template>
<div class="card">
    <img :src="card.thumb" alt="">
    {{card.series}}
</div>
</template>

<script>
export default {
    name: 'CardComponent',
    props:{
        card: Object,
    },
    mounted(){
        console.log(this.cards, 'ricevuto da cardcomponent');
    }

}
</script>

<style lang="scss" scoped>
@import '@/components/main.scss';
    .card{
    @include flex-col;
    padding: 20px;
    img{
        height: 170px;
        width: 170px;
        object-fit: cover;
        object-position: top;
    }
    }
</style>