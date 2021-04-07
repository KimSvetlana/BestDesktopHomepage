<template>
  <div class='main-container' id='main'>
    <HeaderComp/>
    <FeaturesComp/>
    <AboutComp/>
    <WorksComp/>
    <PriceComp/>
    <section class='comments'>
      <div class='row'>
        <div class="col img"></div>
        <div class="col carousel">
          <h2>Trusted By More Than 55M Peoples</h2>
          <CommentCard />
        </div>
      </div>
    </section>
    <NewsComp/>
    <FreeTrialComp/>
    <SubscribeComp/>
    <Footer/>

  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import HeaderComp from './header.vue'
import FeaturesComp from './features.vue'
import AboutComp from './aboutComp.vue'
import WorksComp from './worksComp.vue'
import PriceComp from './priceComp.vue'
import NewsComp from './newsComp.vue'
import FreeTrialComp from './freeTrialComp.vue'
import SubscribeComp from './subscribeComp.vue'
import Footer from './footer.vue'
import CommentCard from './commentCard.vue'
// import Carousel from './carousel.vue'

@Component({
  components: {
    HeaderComp,
    FeaturesComp,
    AboutComp,
    WorksComp,
    PriceComp,
    NewsComp,
    FreeTrialComp,
    SubscribeComp,
    Footer,
    CommentCard
    // Carousel
  }

})
export default class Main extends Vue {}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
   @import '../assets/variables.scss';

  section.comments{
    background: $lightBackgroundColor;
  }
  section.comments .img{
    height: 445px;
    background: url('../assets/images/Image.png') no-repeat;
    background-size: cover;
  }
</style>
