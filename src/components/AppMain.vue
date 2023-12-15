<!-- HTML & VUE3 -->
<template lang="">
    <main>

        <!-- Section 01 -->
        <section class="content">
            <div id="container">
                <!-- Serie -->
                <AppListSeries/>
            </div>
         </section>

         <!-- Section 02 -->
         <section class="cards">
            <div id="container"> 
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

    #container {
        @include my-wrapper();
        @include flex(column,center,start);
    }
    .cards{
        background-color: #0282f9;
    }

    h1{
        padding: 3rem 0;
    }
 
</style>