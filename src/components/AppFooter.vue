<!-- HTM & Vue -->
<template lang="">
    <footer>

        <!-- Meta  -->
         <section class="meta">
            <div id="container">
            <nav id="pastificio">
                <h2>
                    DC COMICS
                </h2>
                <ul>
                    <li><a href="#">Il Pastificio</a></li>
                    <li><a href="#">Grano</a></li>
                    <li><a href="#">Filiera</a></li>
                    <li><a href="#">100 anni di pasta</a></li>
                    <li><a href="#">Sartoria della pasta</a></li>
                </ul>
            </nav>
            <nav id="prodotti">
                <h2>
                    SHOP
                </h2>
                <ul>
                    <li><a href="#">Le classiche</a></li>
                    <li><a href="#">Le Integrali</a></li>
                    <li><a href="#">Le Speciali</a></li>
                    <li><a href="#">Le Biologiche</a></li>
                    <li><a href="#">Le Gluten-free</a></li>
                </ul>
            </nav>
            </div>
         </section>

          <!-- Sign Up Now -->
        <section class="content">
            <div id="container">

            </div>
         </section>

    </footer>
</template>

<!-- JAvaScript -->
<script>
export default {
    // NAme Application
    name: 'AppFoter',
    // Data
    data() {
        return {
            navLinks: [
                {
                    content: 'charters',
                    url: '#',
                    active: false,
                },
                {
                    content: 'comics',
                    url: '#',
                    active: false,
                },
                {
                    content: 'movies',
                    url: '#',
                    active: false,
                },
                {
                    content: 'tv',
                    url: '#',
                    active: false,
                },
                {
                    content: 'games',
                    url: '#',
                    active: false,
                },
                {
                    content: 'collectibles',
                    url: '#',
                    active: false,
                },
                {
                    content: 'videos',
                    url: '#',
                    active: false,
                },
                {
                    content: 'fans',
                    url: '#',
                    active: false,
                },
                {
                    content: 'news',
                    url: '#',
                    active: false,
                },
                {
                    content: 'shop',
                    url: '#',
                    active: false,
                },
            ],
        }
    },
    
}
</script>

<!-- Sass -->
<style lang="scss" scoped>

    // Use StyleSheets
    @use '../scss/partials/variables' as *;
    @use '../scss/partials/mixins' as *;

    footer{
        background-color: $main-color;
        color: white;
    }

    #container {
        @include my-wrapper();
        @include flex(column,center,start);
        top: 50%;
    }
    .meta{
        background-image: url(../assets/img/footer-bg.jpg);
        background-position: center;
    }

    h2{
        padding-bottom: 1.5rem;
    }

    ul{
        list-style-type: none;
        li{
            margin-bottom: 0.5rem;
        }
    }

    a {
        text-decoration: none;
        color: white;
    }

</style>