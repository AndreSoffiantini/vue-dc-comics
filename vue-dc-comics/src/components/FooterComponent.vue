<template>
    <footer id="site_footer">

      <section class="footer_top">
        <div class="container">
          <div class="row">
            <div class="col d-flex">
              <div class="small-col">
                <h2>DC Comics</h2>
                <ul>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                </ul>

                <h2>Shop</h2>
                <ul>
                  <li>Characters</li>
                  <li>Characters</li>
                </ul>

              </div>

              <div class="small-col">
                <h2>DC</h2>
                <ul>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                </ul>
              </div>

              <div class="small-col">
                <h2>Sites</h2>
                <ul>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                  <li>Characters</li>
                </ul>
              </div>

            </div>

            <div class="col"></div>

          </div>
        </div>
      </section>

      <section class="sign_up_socials">

        <div class="container">
          <div class="row">

            <div class="col d-flex align-center">
              <div class="sign_up_btn">
                Sign-up now!
              </div>
            </div>

            <div class="socials col d-flex align-center">
              <h2>Follow Us</h2>
              <img v-for="item in socials" :key="item.id" :src="item.src" alt="">
            </div>

          </div>
        </div>

      </section>

  </footer>
</template>

<script>
export default {
    name: 'HeaderComponent',
    data() {
      return {
        socials: [
          {
            id: 1,
            src: require('@/assets/img/footer-facebook.png')
          },
          {
            id: 2,
            src: require('@/assets/img/footer-twitter.png')
          },
          {
            id: 3,
            src: require('@/assets/img/footer-youtube.png')
          },
          {
            id: 4,
            src: require('@/assets/img/footer-pinterest.png')
          },
          {
            id: 5,
            src: require('@/assets/img/footer-periscope.png')
          },
        ]
      }
    }
}
</script>

<style lang="scss" scoped>

  /* @import '@/assets/sass/variables'; */

  h2 {
    text-transform: uppercase;
    color: white;
  }

  .footer_top {
    background-image: url('@/assets/img/footer-bg.jpg');
    background-size: cover;

  .small-col {
    margin: 3rem 2rem 5rem 0;
  }

    h2 {
      margin: 1rem 0
    }

    ul {
      list-style: none;

      li {
        color: $secondary-light;
      }
    }

    .col:last-child {
      background-image: url('@/assets/img/dc-logo-bg.png');
      background-size: cover;
      background-position: center;
    }
  }

  .sign_up_socials {
    background-color: $secondary;
    padding: 2rem 0;

    .sign_up_btn {
      border: 1px solid $primary;
      padding: 0.75rem;
      color: white;
      text-transform: uppercase;
    }

    .socials {
      
      justify-content: flex-end;

      h2 {
        color: $primary;
        margin: 0 1rem;
      }

      img {
        margin: 0 1rem;

      }

    }
  }

</style>