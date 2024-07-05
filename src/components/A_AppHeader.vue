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

    </header>

</template>

<style lang="scss" scoped>
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
                            border-bottom: 6px solid #0282f9;
                        }
                    }

                    a {
                        color: rgb(151, 151, 151);
                    }
                    
                }
            }
        }
    }
}

</style>
