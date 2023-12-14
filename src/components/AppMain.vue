<template lang="">
    <main>
        <!-- Section 01 -->
        <section class="content">
            <div id="container">
                <h1>
                    Content Gooes Here                    
                </h1>
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
        <!-- Section 03 -->
         <section class="meta">
            <div id="container">
                <h1>
                    Content Gooes Here                    
                </h1>
            </div>
         </section>

    </main>
</template>
<script>
export default {
    name: 'AppMain',
    
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

    .meta{
        background-image: url(../assets/img/footer-bg.jpg);
        height: 300px;
        object-fit: contain;
    }

    h1{
        padding: 3rem 0;
    }
 
</style>