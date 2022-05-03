<template>
    <header id="site_header">
        <div class="container h-100">
            <div class="row h-100">
                <div class="col d-flex align-center">
                    <img src="@/assets/img/dc-logo.png" alt="">
                </div>

                <div class="col d-flex justify-end">
                    <nav class="d-flex align-center unstyled-list h-100">
                        <a href="">Characters</a>
                        <a href="" class="active">Comics</a>
                        <a href="">Movies</a>
                        <a href="">Tv</a>
                        <a href="">Games</a>
                        <a href="">Collectibles</a>
                        <a href="">Videos</a>
                        <a href="">Fans</a>
                        <a href="">News</a>
                        <a href="">Shop</a>
                    </nav>
                </div>
            </div>
        </div>
  </header>
</template>

<script>
export default {
    name: 'HeaderComponent'
}
</script>

<style lang="scss" scoped>

    @import '@/assets/sass/variables';

    header {
        height: 185px;
        padding: 0 3rem;
    }

    nav {
        margin-left: -1rem;
        margin-right: -1rem;

        a {
            text-transform: uppercase;
            text-decoration: none;
            font-weight: 600;
            color: black;
            margin: 0 1rem;
            height: 100%;
            display: flex;
            align-items: center;
            border-bottom: 5px solid transparent;
            
            &.active {
                color: $primary;
                border-bottom-color: $primary;
            }
        }
    }

     

</style>