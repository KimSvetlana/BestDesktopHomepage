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
        <div class="col"></div>
    </div>
    <div class='row'>
      <div class="col"></div>
    </div>
  </section>
  <h1>{{msg}}</h1>
  <button type="button" class="btn btn-primary">Primary</button>
</div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'
import FeaturesItem from './featuresItem.vue'

@Component({
  components: {
    FeaturesItem
  }

})

export default class Main extends Vue {
    @Prop() private msg!: string;
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
    color: #929292;
  }
  .nav-btn{
    padding: 15px 51px;
    text-transform: uppercase;
    color: white;
    background: #0063DD;
    border-radius: 25px;
  }
  .nav-btn:hover{
    border: 2px solid #0063DD;
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
    background-color:#0063DD;
  }
  .btn-trial{
    color:$backgroundButtonColor;
    border:2px solid $backgroundButtonColor;
  }
  .btn-trial:hover{
    color:#0063DD;
    border-color: #0063DD;
  }

  .features {
    background-color: $lightBackgroundColor ;
  }

</style>
