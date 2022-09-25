<template>
  <header> 
    <img src="../../assets/img/dc-logo.png" alt="dc-logo">
    <nav>
        <ul>
            <li>CHARACTERS</li>
            <li>COMICS</li>
            <li>MOVIES</li>
            <li>TV</li>
            <li>GAMES</li>
            <li>COLLECTIBLES</li>
            <li>VIDEOS</li>
            <li>FANS</li>
            <li>NEWS</li>
            <li>SHOP</li>
        </ul>
    </nav>
  </header>
</template>

<script>
export default {
    name: 'HeaderComponent'

}
</script>

<style lang="scss" scoped>
@import '../main.scss';
header{
    @include my-width;
    @include flex-row;
    height: 15vh;
    justify-content: space-between;
    align-items: center;
    font-size: 0.8rem;
    img{
        height: 100%;
    }
    nav ul{
        @include flex-row;
        list-style-type: none;
        li{
            padding-right: 10px;
            &.hover{
                color: $dc-blue;
            }
        }
    }

}



</style>