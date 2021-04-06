<template>
    <section class='container about'>
      <div class='row easy-messag'>
          <div class="col img-wrapper-first">
            <img src="../assets/images/Back1.png" alt=""/>
            <img src="../assets/images/Screen1.png" alt=""/>
          </div>
          <div class="col text-start">
            <h2 class="bannerH2">Easy Messaging</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
            <a class='about-link' href="">Read More<img src="../assets/images/ArrowLeft2.svg"/></a>
          </div>
      </div>
      <div class='row'>
        <div class="col text-start">
          <h2 class="bannerH2">Keep In Touch</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
          <a class='about-link' href="">Read More<img src="../assets/images/ArrowLeft2.svg"/></a>
        </div>
        <div class="col img-wrapper-second">
            <img src="../assets/images/Back1.png" alt=""/>
            <img src="../assets/images/Screen2.png" alt=""/>
        </div>
      </div>
    </section>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component({
  components: {}
})
export default class AboutComp extends Vue {}
</script>

<style lang="scss">
    @import '../assets/variables.scss';

    section.about{
        padding-top: 60px;
        padding-bottom: 116px;
    }

    .about .col{
        margin: auto;
    }

    .about .bannerH2{
        font-weight: 500;
    }
    .about p{
        line-height: 1.5rem;
    }
    .about-link{
        color: $darkBackgroundColor;
        font-weight: 500;
        line-height: 24px;
        text-decoration: none;
        &:hover{
            text-decoration: underline;
        }
        & img{
            margin-left: 15px;
        }
    }
    .easy-messag{
        margin-bottom: 230px;
    }
    .img-wrapper-first{
        position: relative;
        & img:first-child{
            position: absolute;
            top: -100px;
            left: -50px;
        }
        & img:last-child{
            position: relative;
            z-index: 2;
        }
    }
    .img-wrapper-second{
        position: relative;
        & img:first-child{
            position: absolute;
            top: -30px;
            left: 100px;
        }
        & img:last-child{
            position: relative;
            z-index: 2;
        }
    }
</style>
