<template>
<div>
    <ul>
        <h3>Titolo lista</h3>
        <li>Link</li>
        <li>Link</li>
        <li>Link</li>
        <li>Link</li>
        <li>Link</li>
    </ul>

</div>
  
</template>

<script>
export default {
    name: 'linksListComponent'
}
</script>

<style lang="scss" scoped>
@import '@/components/main.scss';
div{
    @include flex-row;
    width: calc(100%/3);
    h3{
        padding: 5px 0px;
        font-size: 0.9rem;
    }
    ul{
        padding: 5px;
    @include flex-col;
    list-style-type: none;
        li{
            color: grey;
            font-size: 0.8rem;
        }

    }
}




</style>