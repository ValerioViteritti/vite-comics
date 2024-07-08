<script>
    export default {
        name:"DcCard",
        // props: [details],
        props: {
            details: Object
        }
    }
</script>

<template>
    <div class="DcCard">
        <div>
            <img :src="details.thumb" alt="descrizione alternativa">
            <h3> {{ details.series }} </h3>
        </div>
        
    </div>
    
   

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.DcCard {
    height: 200px;
    width: 150px;
    


    div {

        img {
        height: 150px;
        width: 150px;
        cursor: pointer;

        }

        h3{
            color: white;
            cursor: pointer;
            margin-top: 10px;
            font-size: 14px;

            
        }

    }

    
}


</style>