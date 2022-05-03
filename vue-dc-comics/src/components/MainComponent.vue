<template>
    <main id="site_main">

      <section class="debug content_section">
        <div class="container">
          <div class="row">
            <div class="col">
              <span>Content goes here</span>
            </div>
          </div>
        </div>
      </section>

      <section class="options_section">
        <div class="container">
          <div class="row">

            <div class="col-20">
              <img src="@/assets/img/buy-comics-digital-comics.png" alt="">
              <span>Digital comics</span>
            </div>

            <div class="col-20">
              <img src="@/assets/img/buy-comics-merchandise.png" alt="">
              <span>DC Merchandise</span>
            </div>

            <div class="col-20">
              <img src="@/assets/img/buy-comics-subscriptions.png" alt="">
              <span>Subscription</span>
            </div>

            <div class="col-20">
              <img src="@/assets/img/buy-comics-shop-locator.png" alt="">
              <span>Comic shop location</span>
            </div>

            <div class="col-20">
              <img src="@/assets/img/buy-dc-power-visa.svg" alt="">
              <span>DC Power VISA</span>
            </div>

          </div>
        </div>
      </section>

  </main>
</template>

<script>
export default {
    name: 'MainComponent'
}
</script>

<style lang="scss" scoped>

@import '@/assets/sass/variables';

  .debug.content_section {
    background-color: $secondary-dark;
    color: white;
    font-size: 200%;
    display: flex;
    align-items: center;
    height: 200px;
  }

  .options_section {
    background-color: $primary;
    padding: 3rem 0;
    color: white;
    /* display: flex;
    align-items: center; */

    .col-20 {
      display: flex;
      align-items: center;

      img {
        max-height: 100px;
      }

      span {
        margin-left: 1rem;
        text-transform: uppercase;
      }

    }
  }

  

</style>