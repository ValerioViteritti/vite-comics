<script>
    export default{
        name: 'FootDcMain',
        data() {
            return {
                DcComics: [
                    {
                        text: 'Character'
                    },
                    {
                        text: 'Comics'
                    },
                    {
                        text: 'Movies'
                    },
                    {
                        text: 'TV'
                    },
                    {
                        text: 'Games'
                    },
                    {
                        text: 'Videos'
                    },
                    {
                        text: 'News'
                    }

                ],

                Shop: [
                    {
                        text: 'Shop DC'
                    },
                    {
                        text: 'Shop DC Collectibles'
                    }

                ],

                Dc: [
                    {
                        text: 'Terms Of Use'
                    },
                    {
                        text: 'Privacy policy (New)'
                    },
                    {
                        text: 'Ad Choices'
                    },
                    {
                        text: 'Advertising'
                    },
                    {
                        text: 'Jobs'
                    },
                    {
                        text: 'Subscriptions'
                    },
                    {
                        text: 'Talent Workshops'
                    },
                    {
                        text: 'CPSC Certificates'
                    },
                    {
                        text: 'Ratings'
                    },
                    {
                        text: 'Shop Help'
                    },
                    {
                        text: 'Contact Us'
                    }

                ],

                Sites: [
                    {
                        text: 'DC'
                    },
                    {
                        text: 'MAD Magazine'
                    },
                    {
                        text: 'DC Kids'
                    },
                    {
                        text: 'DC Universe'
                    },
                    {
                        text: 'DC Power Visa'
                    }

                ]

            }
        }
    }

</script>

<template>
    <div class="container">
        <div class="row">
            <div id="list">
                <h3>DC COMICS</h3>
                    <ul v-for="(DcComics, index) in DcComics" :key="index">
                        <li>{{ DcComics.text }}</li>
                    </ul>

                <h3>SHOP</h3>
                    <ul v-for="(Shop, index) in Shop" :key="index">
                        <li>{{ Shop.text }}</li>
                    </ul>

                <h3>DC</h3>
                    <ul v-for="(Dc, index) in Dc" :key="index">
                        <li>{{ Dc.text }}</li>
                    </ul>

                <h3>SITES</h3>
                    <ul v-for="(Sites, index) in Sites" :key="index">
                        <li>{{ Sites.text }}</li>
                    </ul>

                
            </div>
            <div id="img">
                <img src="../assets/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
    

</template>

<style lang="scss" scoped>
.container {
  height: calc((100vh / 23) * 10);
  background-image: url('../assets/footer-bg.jpg');
  background-size: cover;

  .row {
    width: 80%;
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;

    div {
      height: 100%;

      &#list{
        height: 80%;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        gap: 10px;
        margin-left: 0;
        

        h3{
            color: white;
            font-size: 1.5rem;
            margin-left: 0;
            margin-top: 5px;
            margin-bottom: 5px;
        }

        ul{
            list-style-type: none;
            color: #949596;
            margin-left: 0;

            li {
                font-size: 0.8rem;
                margin-right: 30px;
                cursor: pointer;
            
            }
        }
      }
    }

    #img {
      position: relative;
      width: 600px;
      height: 500px;

      img {
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        object-fit: cover;
      }
    }
  }
}
</style>
