<template>
<footer>
    <div>
        <linksListComponent/>
        <linksListComponent/>
        <linksListComponent/>
        <linksListComponent/>
    </div>
        <img src="@/assets/img/dc-logo-bg.png" alt="dc footer logo">
    



</footer>
</template>


<script>

import linksListComponent from '@/components/footer/linksListComponent.vue'

export default {
    name: 'MiddleFooter',
    components:{ linksListComponent}

}
</script>

<style lang="scss" scoped>
@import '@/components/main.scss';
footer{
    @include my-width;
    @include flex-row;
    max-height: 46vh;
    width: 100vw;
    background-image: url(@/assets/img/footer-bg.jpg);
    background-size: cover;
    justify-content: space-between;
    overflow-y: hidden;
    div{
        @include flex-row;
        flex-grow: 1;
        flex-wrap: wrap;
        color: white;
        ul{
            @include flex-col;
            list-style-type: none;
        }

    }
    img{
    width: 50%;
    height: 100%;
    transform: translateY(-70px);
    flex-grow: 0;
    }
}


</style>