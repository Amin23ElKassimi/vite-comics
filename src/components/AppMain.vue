<!-- HTML & VUE3 -->
<template lang="">
    <main>
        <!-- Section 01 -->
        <section id="bg-teentitans">
            <img src="../assets/img/jumbotron.jpg" alt="">
        </section>
        <!-- Section 01 -->
        <section class="container">
            <!-- Serie -->
            <AppListSeries/>
        </section>
         <!-- Section 02 -->
         <section class="cards">
            <div class="container"> 
                <h1>
                    Content Gooes Here                    
                </h1>
            </div>
         </section>
    </main>
</template>

<!-- JavaScript -->
<script>

// Import Del figlio
import AppListSeries from './AppListSeries.vue';

export default {

    name: 'AppMain',

    // Dichiarare componet
    components: {
        AppListSeries
    }
    
}
</script>

<!-- Sass -->
<style lang="scss" scoped>

    // Use StyleSheets
    @use '../scss/partials/variables' as *;
    @use '../scss/partials/mixins' as *;

    main{
        background-color: $main-color;
        color: white;
    }

    #bg-teentitans {
        width: 100%;
        object-fit: cover;
        img{
            height: 500px;
            width: 100%;
        }
    }
    .container {
        @include my-wrapper();
        @include flex(row, space-evenly, stretch);
        margin: 0 auto;
        flex-wrap: wrap;
    }
    .cards{
        background-color: #0282f9;
    }

    h1{
        padding: 3rem 0;
    }
 
</style>