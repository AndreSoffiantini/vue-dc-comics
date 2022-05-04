<template>
    <header id="site_header">
        <div class="container h-100">
            <div class="row h-100">
                <div class="col d-flex align-center">
                    <img src="@/assets/img/dc-logo.png" alt="">
                </div>

                <div class="col d-flex justify-end">
                    <Navbar/>
                </div>
            </div>
        </div>
  </header>
</template>

<script>

import Navbar from '@/components/NavbarComponent.vue'

export default {
    name: 'HeaderComponent',
    components: {
        Navbar
    }
}
</script>

<style lang="scss" scoped>

    header {
        height: 185px;
    }     

</style>