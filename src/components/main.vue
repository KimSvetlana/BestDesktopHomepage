<template>
<div class='main-container'>
  <header>
    <nav class="header-nav navbar navbar-expand-lg navbar-light">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">AppSon</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Features</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Pricing</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Pages</a>
          </li>
        </ul>
          <button class="btn nav-btn">Sign up</button>
      </div>
      </div>
    </nav>
    <section class=" header-content container">
      <div class="row align-items-start">
        <div class="col">
          <h1 class='header-title'>Best Desktop App for You</h1>
          <p class='header-text'>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor<br>
           incididunt ut labore et dolore magna aliqua. adipisicing elit, sed do eiusmod tempor <br>
           incididunt ut labore et dolore magna aliqua.</p>
          <button class='btn btn-download'>Download</button>
          <button  class='btn btn-trial'>Free Trial</button>
          <div class='phones'>
            <img src="../assets/images/Phone1.png"/>
          </div>
        </div>
      </div>
    </section>
  </header>

  <section class='features'>
    <div class="row align-items-center">
      <div class="col">
        <img src='../assets/images/Icon1.png' class='item-img' />
        <FeaturesItem itemHeader="Analysis"/>
      </div>
      <div class="col">
        <img src='../assets/images/Icon2.png' class='item-img' />
        <FeaturesItem itemHeader="Clean Design"/>
      </div>
      <div class="col">
        <img src='../assets/images/Icon3.png' class='item-img' />
        <FeaturesItem itemHeader="Messaging" />
      </div>
    </div>
  </section>

  <section class='about'>
    <div class='row'>
        <div class="col">
          <img src="../assets/images/Screen1.png" alt="">
        </div>
        <div class="col">
          <h2>Easy Messaging</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
          <a href="">Read More</a>
        </div>
    </div>
    <div class='row'>
      <div class="col">
        <h2>Keep In Touch</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
         <a href="">Read More</a>
      </div>
      <div class="col">
        <img src="../assets/images/Screen2.png" alt="">
      </div>
    </div>
  </section>

  <section class='works'>
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
  </section>

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
import FeaturesItem from './featuresItem.vue'
import WorksItem from './worksItem.vue'
import PriceItem from './priceItem.vue'
import CommentCard from './commentCard.vue'
// import Carousel from './carousel.vue'

@Component({
  components: {
    FeaturesItem,
    WorksItem,
    PriceItem,
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
  header{
    min-height: 1029px;
    background: url('../assets/images/headerBackground.png');
    background-position: center;
    // background: linear-gradient(206.38deg, #0F7BFF 8.31%, #0063DD 61.03%);
    box-shadow: -7px -7px 32px rgba(0, 30, 67, 0.06);
  }
  header .navbar{
    padding: 0;
  }

  .navbar-light .navbar-brand{
    display: block;
    width: 179px;
    height: 100px;
    color: white;
    background-color: $backgroundButtonColor;
    border-radius: 0px 0px 21.5px 21.5px;
    font-weight: bold;
    font-size: 36px;
    line-height: 45px;
  }

  .navbar-light .navbar-nav .nav-link {
    text-transform: uppercase;
    // color: rgba(0, 0, 0, 0.55);
  }

  ul.navbar-nav .nav-item .nav-link:hover{
    text-decoration: underline;
  }
  ul.navbar-nav .nav-item .nav-link.active{
    color: #0F7CFF;
  }

  .header-text{
    line-height: 169%;
    color: #929292;
  }
  .nav-btn{
    padding: 15px 51px;
    text-transform: uppercase;
    color: white;
    background: $darkBackgroundColor;
    border-radius: 25px;
  }
  .nav-btn:hover{
    border: 2px solid $darkBackgroundColor;
    background: none;
  }
  ul.navbar-nav {
    margin-left: auto;
  }
  .btn-download,
  .btn-trial{
    padding: 14px 44px;
    border-radius: 25px;
  }
  .btn-download{
    color:white;
    margin-right: 30px;
    background-color: $backgroundButtonColor;
  }
  .btn-download:hover{
    background-color: $darkBackgroundColor;
  }
  .btn-trial{
    color:$backgroundButtonColor;
    border:2px solid $backgroundButtonColor;
  }
  .btn-trial:hover{
    color: $darkBackgroundColor;
    border-color: $darkBackgroundColor;
  }

  .features {
    background-color: $lightBackgroundColor ;
  }

  section.works{
    background-color: $lightBackgroundColor;
  }

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
