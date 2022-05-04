<template>
    <section class="banner_section">
        <div class="container">
          <div class="row">

            <div class="col-20" v-for="item in banner" :key="item.id">
              <img :src="item.src" alt="">
              <span>{{item.text}}</span>
            </div>

          </div>
        </div>
      </section>
</template>

<script>
export default {
    name:'BannerComponent',
    data() {
      return {
        banner: [
          {
            id: 1,
            src: require('@/assets/img/buy-comics-digital-comics.png'),
            text: 'Digital comics'
          },
          {
            id: 2,
            src: require('@/assets/img/buy-comics-merchandise.png'),
            text: 'DC Merchandise'
          },
          {
            id: 3,
            src: require('@/assets/img/buy-comics-subscriptions.png'),
            text: 'Subscription'
          },
          {
            id: 4,
            src: require('@/assets/img/buy-comics-shop-locator.png'),
            text: 'Comic shop location'
          },
          {
            id: 5,
            src: require('@/assets/img/buy-dc-power-visa.svg'),
            text: 'DC Power VISA'
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>

/* @import '@/assets/sass/variables'; */

    .banner_section {
    background-color: $primary;
    padding: 4rem 0;
    color: white;

    .col-20 {
      display: flex;
      align-items: center;
      justify-content: center;

      img {
        max-height: 75px;
      }

      span {
        margin-left: 1rem;
        text-transform: uppercase;
      }

    }
  }

</style>