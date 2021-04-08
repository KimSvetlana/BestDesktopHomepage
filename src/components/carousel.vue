<template>
<div class="comments-carousel">
    <b-carousel
      id="comments-carousel"
      controls
      indicators
    >
    <!-- Slide with blank fluid image to maintain slide aspect ratio -->
      <b-carousel-slide img-blank img-width="1024" img-height="480">
        <div class='row carousel-slide'>
          <div class='col'><CommentCard/></div>
          <div class='col'><CommentCard/></div>
          <div class='col'><CommentCard/></div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide img-blank img-width="1024" img-height="480">
        <div class='row carousel-slide'>
          <div class='col'><CommentCard/></div>
          <div class='col'><CommentCard/></div>
          <div class='col'><CommentCard/></div>
        </div>
      </b-carousel-slide>
      <b-carousel-slide img-blank img-width="1024" img-height="480">
        <div class='row carousel-slide'>
          <div class='col'><CommentCard/></div>
          <div class='col'><CommentCard/></div>
          <div class='col'><CommentCard/></div>
        </div>
      </b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import CommentCard from './commentCard.vue'

@Component({
  components: {
    CommentCard
  }
})
export default class Carousel extends Vue {}
</script>
<style lang="scss">
.comments-carousel .carousel-control-next,
.comments-carousel .carousel-control-prev{
  display: none;
}
.comments-carousel .carousel-indicators{
  height: 20px;
  top: 275px;
  justify-content: start;
  margin-left: auto;
}
.carousel-indicators::before{
  content:"";
  width: 40px;
  height: 12px;
  border-radius: 6px;
  background-color:#0063DD;
}
.comments-carousel .carousel-indicators li{
  width:12px;
  height: 12px;
  border-radius: 50%;
  border: 1.6px solid #0063DD;
  margin-left: 8px;
  &:active{
    background-color: #0063DD;
    border-color:#0063DD; ;
  }
  & .active{
    background-color: #0063DD;
  }
}
  #comments-carousel .carousel-caption{
    top: 0%;
    left: 0%;
    color:black;
  }
  #comments-carousel .carousel-slide {
    flex-wrap: nowrap !important;
  }
  @media screen and (min-width: 375px) and (max-width: 540px) {
     #comments-carousel .carousel-slide{
        flex-wrap: wrap !important;
      }
      #comments-carousel .carousel-item{
        height: 220px;
      }
  }
</style>
