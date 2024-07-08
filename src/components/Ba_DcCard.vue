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
    <div class="Dc-card">
        <img :src="details.thumb" alt="descrizione alternativa">
        <h3> {{ details.series }} </h3>
    </div>
    
   

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;


</style>