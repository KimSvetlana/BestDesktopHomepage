<template>
  <div class='main-container' id='main'>
    <HeaderComp/>
    <FeaturesComp/>
    <AboutComp/>
    <WorksComp/>
    <PriceComp/>
    <!-- <section class='works'>
      <h2>How Does It Works?</h2>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet.</p>
      <div class='row'>
        <div class="col">
          <img src="../assets/images/Icon4.png" alt="">
          <WorksItem itemHeader="Create An Account"/>
        </div>
        <div class="col">
          <img src="../assets/images/Icon5.png" alt="">
          <WorksItem itemHeader="Confirm Email"/>
        </div>
        <div class="col">
          <img src="../assets/images/Icon6.png" alt="">
          <WorksItem itemHeader="See Results"/>
        </div>
      </div>
    </section>

    <section class="price">
      <div class='row'>
        <div class="col">
          <h2>Pricing Plan</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet.</p>
          <button class='btn'>Monthly</button>
          <button class='btn'>Yearly</button>
        </div>
        <div class="col">
          <img src="../assets/images/Icon7.png" alt="">
          <PriceItem priceHeader="Premium" itemCost="49.00"/>
        </div>
        <div class="col">
          <img src="../assets/images/Icon8.png" alt="">
          <PriceItem priceHeader="Standart" itemCost="19.00"/>
        </div>
      </div>
    </section>

    <section class='comments'>
      <div class='row'>
        <div class="col img"></div>
        <div class="col carousel">
          <h2>Trusted By More Than 55M Peoples</h2>
          <CommentCard />

        </div>
      </div>
    </section>

    <section class='free-trial'>
      <div class='row'>
        <div class= "col">
          <h2>Try 30 Days Free Trial</h2>
          <p>No credit card reauired</p>
        </div>
        <div class= "col">
          <button class="btn free-trial-btn">Get Stared
            <img src="../assets/images/ArrowLeft.svg"/>
          </button>
        </div>
      </div>
    </section>

    <section  class='subscribe'>
      <h2 class='logo'>AppSon</h2>
      <div class="input-group mb-3">
        <input type="text" class="form-control" placeholder="Enter your Email" aria-label="Subscribe" aria-describedby="button-addon2">
        <button class="btn btn-outline-secondary btn-subscribe" type="button" id="button-addon2">Subscribe</button>
      </div>
    </section> -->

    <footer>
      <div class='row'>
        <div class='col copiraight'>
          <p>© 2018 Copyright, All Rights Reserved by AppSon</p>
        </div>
        <div class='col'>
          <nav class="nav justify-content-end">
            <a class="nav-link active" aria-current="page" href="#">Active</a>
            <a class="nav-link" href="#">Link</a>
            <a class="nav-link" href="#">Link</a>
            <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
          </nav>
        </div>
        <div class='col'>
          <ul class='footer-social-list'>
                  <li>
                      <a href="#">
                          <img src="../assets/images/Facebook.svg"  width="30" height="30">
                      </a>
                  </li>
            <li>
                      <a href="#">
                        <img src="../assets/images/Twitter.svg"  width="30" height="30">
                      </a>
                  </li>
                  <li>
                      <a href="#">
                          <img src="../assets/images/YouTube.svg" alt="Equiteez" width="30" height="30">
                      </a>
                  </li>
          </ul>
        </div>
      </div>
    </footer>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import HeaderComp from './header.vue'
import FeaturesComp from './features.vue'
import AboutComp from './aboutComp.vue'
import WorksComp from './worksComp.vue'
import PriceComp from './priceComp.vue'
import CommentCard from './commentCard.vue'
// import Carousel from './carousel.vue'

@Component({
  components: {
    HeaderComp,
    FeaturesComp,
    AboutComp,
    WorksComp,
    PriceComp,
    CommentCard
    // Carousel
  }

})
export default class Main extends Vue {
  // @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
   @import '../assets/variables.scss';

  section.comments .img{
    height: 445px;
    background: url('../assets/images/Image.png') no-repeat;
    background-size: cover;
  }

  section.free-trial{
    background-color: $lightBackgroundColor;
  }
  .free-trial-btn{
    padding: 14px 68px;
    color:white;
    border-radius: 25px;
    background-color: $backgroundButtonColor;
  }

  section.subscribe{
    padding: 50px;
    background-color: $backgroundButtonColor;
  }
  .subscribe input {
    background-color: $darkBackgroundColor ;
    border-radius: 25px 0 0 25px;
  }
  .subscribe input::placeholder{
    color:white;
  }
  .subscribe .btn-subscribe{
    background-color: white;
    color:$darkBackgroundColor;
    border-radius: 0 25px 25px 0;
  }

  footer {
    background-color: $darkBackgroundColor;
  }
</style>
