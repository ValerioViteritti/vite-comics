<script>
    export default{
        name: 'DcMain',
    }

</script>

<template>
    <div class="container">
        <div class="row">
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
        </div>
    </div>

</template>

<style lang="scss" scoped>
div.container{
    height: calc((100vh / 23) * 4);
    background-color: #0282f9;

    div.row{
        width: 80%;

        div{
            width: calc(100% / 5);
        }
    }
}

</style>