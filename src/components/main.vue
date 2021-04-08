<template>
  <div class='main-container' id='main'>
    <HeaderComp/>
    <FeaturesComp/>
    <AboutComp/>
    <WorksComp/>
    <PriceComp/>
    <CommentsComp/>
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
import CommentsComp from './commentsComp.vue'
import NewsComp from './newsComp.vue'
import FreeTrialComp from './freeTrialComp.vue'
import SubscribeComp from './subscribeComp.vue'
import Footer from './footer.vue'

@Component({
  components: {
    HeaderComp,
    FeaturesComp,
    AboutComp,
    WorksComp,
    PriceComp,
    CommentsComp,
    NewsComp,
    FreeTrialComp,
    SubscribeComp,
    Footer
  }

})
export default class Main extends Vue {}
</script>
