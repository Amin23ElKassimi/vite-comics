<template lang="">
    <header>
        <div id="container">
            <section class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </section>
            <nav class="navbar">
                <ul>
                    <li v-for="(link, index) in navLinks" >
                    {{ link.content}}
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>
<script>
export default {
    name: 'AppHeader',
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
<style lang="scss" scoped>

    // Use StyleSheets
    @use '../scss/partials/variables' as *;
    @use '../scss/partials/mixins' as *;


    #container {
        @include my-wrapper();
        @include flex(row,space-between,center);
    }

    ul {
        @include flex(row,space-between,center);
        list-style-type:none ;
    }

    li{
        font-size: 1.2rem;
        padding: 2rem 1rem;
        &:hover{
            color: blue;
            background-color: antiquewhite;
        }
    }
    
</style>