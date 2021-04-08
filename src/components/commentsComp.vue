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
   @media screen and (max-width: 1219px) {
    .comments .carousel{
      padding-top: 30px;
    }
    .comments .col-7 {
      flex: auto;
      width: 100%
    }
    section.comments .img{
      background: none;
    }
    .comments .row{
      height: 400px;
    }
  }
   @media screen and (min-width: 375px) and (max-width: 680px) {
     .comments .col-5{
        display: none;
        flex: auto;
        width: 100%;
        height: 0;
     }
     .comments .carousel{
        padding-top: 10px;
        padding-left: 25px;
      & h2{
          text-align: center;
          font-weight: bold;
          margin-bottom: 10px;
          font-size:24px;
      }
    }
    #comments-carousel .carousel-caption .row{
      display: initial;
    }
   }
</style>
