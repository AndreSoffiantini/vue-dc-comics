<template>
    <main id="site_main">

      <Jumbotron/>

      <section class="comics_section">
        <div class="container">

          <div class="primary-btn" id="current_series_btn" >Current series</div>

          <Comics/>

          <div class="primary-btn" id="load_more_btn">Load more</div>

        </div>
      </section>

      <Banner/>

  </main>
</template>

<script>
import Jumbotron from '@/components/JumbotronComponent';
import Comics from '@/components/ComicsComponent';
import Banner from '@/components/BannerComponent';

export default {
    name: 'MainComponent',
    components: { 
      Banner,
      Jumbotron,
      Comics
    }
}
</script>

<style lang="scss" scoped>

/* @import '@/assets/sass/variables'; */

  .comics_section {
    background-color: $secondary-dark;
    padding-bottom: 2rem;
    
    .container {
      position: relative;

      .primary-btn {
        background-color: $primary;
        color: white;
        text-transform: uppercase;
      }

      #current_series_btn {
        font-size: 1.5rem;
        padding: 0.5rem 1rem;
        font-weight: 600;
        position: absolute;
        transform: translate(-10px, -50%);
      }

      #load_more_btn {
        width: fit-content;
        margin: auto;
        padding: 0.5rem 2rem;
      }
    }
  }

</style>