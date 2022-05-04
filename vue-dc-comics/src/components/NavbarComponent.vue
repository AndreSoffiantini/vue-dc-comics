<template>
    <nav class="d-flex align-center unstyled-list h-100">
        <a v-for="(item,index) in navbar" v-bind:key="index" :class="item.active ? 'active' : ''">{{item.text}}</a>
    </nav>
</template>

<script>
export default {
    name: 'NavbarComponent',
    data() {
    return {
      navbar: [
  {
	text: 'Characters',
	active: false,
  },
  {
	text: 'Comics',
	active: true,
  },
  {
	text: 'Movies',
	active: false,
  },
  {
	text: 'TV',
	active: false,
  },
  {
	text: 'Games',
	active: false,
  },
  {
	text: 'Collectibles',
	active: false,
  },
  {
	text: 'Videos',
	active: false,
  },
  {
	text: 'Fans',
	active: false,
  },
  {
	text: 'News',
	active: false,
  },
  {
	text: 'Shop',
	active: false,
  }
      ]

    }
  }
}
</script>

<style lang="scss" scoped>

  @import '@/assets/sass/variables';

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