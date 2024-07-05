<script>
export default {
  name: 'AppFooter',
    data() {
        return {
            links: [
                {
                image: 'src/assets/footer-facebook.png',
                alt: 'ICONA FACEBOOK'
                },
                {
                image: 'src/assets/footer-twitter.png',
                alt: 'ICONA TWITTER'
                },
                {
                image: 'src/assets/footer-youtube.png',
                alt: 'ICONA YOUTUBE'
                },
                {
                image: 'src/assets/footer-pinterest.png',
                alt: 'ICONA PINTEREST'
                },
                {
                image: 'src/assets/footer-periscope.png',
                alt: 'ICONA PERISCOPE'
                }
                
            ]
        };
    }
};
</script>


<template>
  <footer>
    <div class="container">
      <div class="row">
        <button>SIGN-UP NOW!</button>
        <div>
          <a href="#">FOLLOW US</a>
          <div v-for="(link, index) in links" :key="index">
            <img :src="link.image" :alt="link.alt">
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
    height: calc((100vh / 23) * 3);
    background-color: #303030;
    z-index: 1000;

    div.container {
        height: 100%;
        width: 80%;

        div.row {
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;

            > div{
                display: flex;
                align-items: center;
                gap: 15px;
            }

            button{
                margin: 0;
                padding: 10px;
                color: white;
                background-color: #303030;
                border: 2px solid #0282f9;
                cursor: pointer;
            }

            a{
                color: #0282f9;
                font-weight: bold;
            }

            div {
                margin: 0;

                img{
                    cursor: pointer;
                }
            }

        }
    }

}

</style>