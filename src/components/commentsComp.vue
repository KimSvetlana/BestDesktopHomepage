<template>
    <section class='comments'>
      <div class='row'>
        <div class="col-5 img"></div>
        <div class="col-7 carousel">
          <h2 class='bannerH2'>Trusted By More Than 55M Peoples</h2>
          <Carousel/>
        </div>
      </div>
    </section>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Carousel from './carousel.vue'

@Component({
  components: {
    Carousel
  }

})
export default class CommentsComp extends Vue {}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
   @import '../assets/variables.scss';

  section.comments{
    box-sizing: border-box;
    background: $lightBackgroundColor;
    max-height: 601px;
  }
  section.comments .img{
    background: url('../assets/images/Image.png') no-repeat;
  }
  .comments .carousel{
        padding-top: 113px;
        padding-left: 80px;
      & h2{
          text-align: start;
          font-weight: bold;
          margin-bottom: 20px;
      }
  }
</style>
