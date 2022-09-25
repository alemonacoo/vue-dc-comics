<template>
<div>
    <ul>
        <li>
            <img src="../../assets/img/buy-comics-digital-comics.png" alt="">
            <p>Descrizione</p>
        </li>
        <li>
            <img src="../../assets/img/buy-comics-merchandise.png" alt="">
           
            <p>Descrizione</p>
        </li>
                <li>
            <img src="../../assets/img/buy-comics-subscriptions.png" alt="">
            <p>Descrizione</p>
        </li>        <li>
            <img src="../../assets/img/buy-comics-shop-locator.png" alt="">
            <p>Descrizione</p>
        </li>
                <li>
            <img src="../../assets/img/buy-dc-power-visa.svg" alt="">
            <p>Descrizione</p>
        </li>
        
    </ul>

</div>
</template>

<script>
export default {
    name: 'TopFooter'

}
</script>

<style lang="scss" scoped>
@import '@/components/main.scss';
div{
    @include my-width;
    @include flex-row;
    background-color: $dc-blue;
    ul{
        @include flex-row;
        list-style-type: none;
        justify-content: space-evenly;
        li{
        @include flex-row;
        align-items: center;
        font-size: 0.8rem;
        color: white;
        }
        li img{
            height: 40%;
            width: auto;    
            padding-right: 10px;        
        }
    }
 
}


</style>