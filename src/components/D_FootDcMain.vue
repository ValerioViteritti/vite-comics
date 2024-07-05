<script>
    export default{
        name: 'FootDcMain',
    }

</script>

<template>
    <div class="container">
        <div class="row">
            <div>
                
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
    }

    #img {
      position: relative;
      width: 600px;
      height: 600px;
      z-index: 0;

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
