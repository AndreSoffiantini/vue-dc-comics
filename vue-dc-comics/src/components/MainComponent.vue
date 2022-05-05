<template>
    <main id="site_main">

      <Jumbotron/>

      <ComicsSection/>

      <Banner/>

  </main>
</template>

<script>
import Jumbotron from '@/components/JumbotronComponent';
import ComicsSection from '@/components/ComicsSectionComponent';
import Banner from '@/components/BannerComponent';

export default {
    name: 'MainComponent',
    components: { 
      Banner,
      Jumbotron,
      ComicsSection
    }
}
</script>

