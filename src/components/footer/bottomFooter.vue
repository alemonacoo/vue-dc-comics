<template>
<footer>
    <button>SIGN UP NOW!</button>
    <div>
        <h3>FOLLOW US</h3>
        <img src="@/assets/img/footer-facebook.png" alt="">
        <img src="@/assets/img/footer-periscope.png" alt="">
        <img src="@/assets/img/footer-pinterest.png" alt="">
        <img src="@/assets/img/footer-twitter.png" alt="">
        <img src="@/assets/img/footer-youtube.png" alt="">
    </div>


</footer>
</template>

<script>
export default {
    name: 'BottomFooter'

}
</script>

<style lang="scss" scoped>
@import '@/components/main.scss';
footer{
    @include my-width;
    @include flex-row;
    justify-content: space-between;
    align-items: center;
    min-height: 10vh;
    background-color: rgb(48,48,48);
    button{
        background-color: rgb(48,48,48);
        color: white;
        border-radius: none;
        border-color: $dc-blue;
        padding: 7px;
            font-size: 0.8rem;

    }
    div{
        @include flex-row;
        align-items: center;
        h3{
            color: $dc-blue;
            font-size: 0.8rem;
        }
        img{
            padding-left: 10px;
            width: 40px;
            
        }

    }



}


</style>