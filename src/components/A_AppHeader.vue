<script>
    export default{
        name: 'AppHeader',
        data() {
            return {
                links:[
                    {
                        text: 'CHARACTERS'
                    },
                    {
                        text: 'COMICS'
                    },
                    {
                        text: 'MOVIES'
                    },
                    {
                        text: 'TV'
                    },
                    {
                        text: 'GAMES'
                    },
                    {
                        text: 'COLLECTIBLES'
                    },
                    {
                        text: 'VIDEOS'
                    },
                    {
                        text: 'FANS'
                    },
                    {
                        text: 'NEWS'
                    },
                    {
                        text: 'SHOP'
                    },
                ]
            }
        }
    }

</script>

<template>
    <header>
        <nav>
            <div class="container">
                <div class="row">
                    <img src="../assets/dc-logo.png" alt="">
                    <div id="linkNav">
                        <div v-for="(links, index) in links" :key="index" >
                            <a href="#">
                                {{ links.text }}
                            </a>
                        </div>

                        
                    </div>

                </div>
            </div>
        </nav>
        <div class="jumbotron">
            <div class="current">CURRENT SERIES</div>
        </div>

    </header>

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
header{
    

    nav{

        div.container{
            height: calc((100vh / 23) * 3);
            
            

            div.row{
                width: 80%;
                height: 100%;
                display: flex;
                justify-content: space-between;
                align-items: center;

                img{
                    margin: 0;
                    height: 70%;

                }
                div#linkNav{
                    height: 100%;
                    margin: 0;
                    display: flex;
                    align-items: center;
                    gap: 30px;

                    div{
                        height: 100%;
                        display: flex;
                        align-items: center;

                        &:hover{
                            border-bottom: 6px solid $primary;
                        }
                    }

                    a {
                        color: rgb(151, 151, 151);
                    }
                    
                }
            }
        }
    }
    .jumbotron{
        background-image: url(src/assets/jumbotron.jpg);
        background-size: cover;
        height: calc((100vh / 23) * 9);
        width: 100%;
        position: relative;

        .current{
            position: absolute;
            top: 90%;
            left: 22%;
            color: white;
            background-color: $primary;
            width: 200px;
            text-align: center;
            margin: 20px 0;
            padding: 10px;
            cursor: pointer;
            }
    }
}

</style>
