<script>
    export default{
        name: 'AppFooter',
    }

</script>

<template>
    <footer>
        <div class="container">
            <div class="row">
                <div>XXX</div>
                <div>VVV</div>
            </div>
        </div>


    </footer>

</template>

<style lang="scss" scoped>
footer{
    height: calc((100vh / 23) * 3);
    background-color: #303030;
    div.container{

        width: 80%;

        div.row{
            display: flex;
            justify-content: space-between;

            div{
                margin: 0;

            }

        }
    }

}

</style>