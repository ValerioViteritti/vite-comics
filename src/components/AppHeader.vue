<script>
    export default{
        name: 'AppHeader',
    }

</script>

<template>
    <header>
        <nav>
            <div class="container">
                <div class="row">
                    <img src="../assets/dc-logo.png" alt="">
                    <div></div>

                </div>
            </div>
        </nav>

    </header>

</template>

<style lang="scss" scoped>
header{
    height: calc((100% / 23) * 3);

    nav{

        div.container{
            width: 80%;
            

            div.row{
                display: flex;
                justify-content: space-between;

                img{

                }
                div{
                    
                }
            }
        }
    }
}

</style>
