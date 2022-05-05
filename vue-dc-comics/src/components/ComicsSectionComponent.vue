<template>
    <section class="comics_section">
        <div class="container">

          <div class="primary-btn" id="current_series_btn" >Current series</div>

          <ComicsList/>

          <a href="#" class="primary-btn" id="load_more_btn">Load more</a>

        </div>
      </section>
</template>

<script>

import ComicsList from "@/components/ComicsListComponent.vue"

export default {
    name: 'ComicsSectionComponent',
    components: {
        ComicsList
    }
}
</script>

<style lang="scss" scoped>

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
        display: block;
        margin: auto;
        padding: 0.5rem 2rem;
        text-decoration: none;
      }
    }
  }

</style>