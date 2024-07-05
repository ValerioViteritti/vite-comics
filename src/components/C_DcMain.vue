<script>
    export default{
        name: 'DcMain',
        data(){
            return {
                links:[
                    {
                        image: "src/assets/buy-comics-digital-comics.png",
                        text: "DIGITAL COMICS"
                    },
                    {
                        image: "src/assets/buy-comics-merchandise.png",
                        text: "DC MERCHANDISE"
                    },
                    {
                        image: "src/assets/buy-comics-subscriptions.png",
                        text: "SUBSCRIPTION"
                    },
                    {
                        image: "src/assets/buy-comics-shop-locator.png",
                        text: "COMIC SHOP LOCATOR"
                    },
                    {
                        image: "src/assets/buy-dc-power-visa.svg",
                        text: "DC POWER VISA"
                    },
                ]
            }

        }
    }


</script>

<template>
    <div class="container">
        <div class="row">
            <div v-for="(links, index) in links" :key="index">
                <img :src="links.image" alt="Logo Digital">
                <span> {{ links.text }} </span>
            </div>
            
        </div>
    </div>

</template>

<style lang="scss" scoped>
div.container{
    height: calc((100vh / 23) * 4);
    background-color: #0282f9;

    div.row{
        width: 80%;
        display: flex;
        height: 100%;

        div{
            width: calc(100% / 5);
            color: white;
            display: flex;
            align-items: center;

            img{
                width: 50px;
            }

            span{
                cursor: pointer;
            }
        }

        
    }
}

</style>