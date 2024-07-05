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
    

    nav{

        div.container{
            height: calc((100vh / 23) * 3);
            
            

            div.row{
                width: 80%;
                display: flex;
                justify-content: space-between;
                align-items: center;

                img{
                    margin: 0;

                }
                div{
                    margin: 0;
                    
                }
            }
        }
    }
}

</style>
