<template>
    <main id="site_main">

      <Jumbotron/>

      <section class="debug content_section">
        <div class="container">
          <div class="row">
            <div class="col">
              <span>Content goes here</span>
            </div>
          </div>
        </div>
      </section>

      <Banner/>

  </main>
</template>

<script>
import Jumbotron from '@/components/JumbotronComponent'
import Banner from '@/components/BannerComponent';

export default {
    name: 'MainComponent',
    components: { 
      Banner,
      Jumbotron
    }
}
</script>

<style lang="scss" scoped>

/* @import '@/assets/sass/variables'; */

  .debug.content_section {
    background-color: $secondary-dark;
    color: white;
    font-size: 200%;
    display: flex;
    align-items: center;
    height: 200px;
  }

</style>