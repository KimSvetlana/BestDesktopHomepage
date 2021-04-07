<template>
    <section class='container about'>
      <div class='row paddingRow easy-messag'>
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
      <div class='row paddingRow keep-in'>
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
        margin-top: 35px;
        margin-bottom: 30px;
    }
    .about p{
        line-height: 1.5rem;
        margin-bottom: 37px;
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
        & .col{
            padding-left: 70px;
        }
    }
    .img-wrapper-first{
        position: relative;
        & img:first-child{
            position: absolute;
            top: -110px;
            left: -65px;
        }
        & img:last-child{
            position: relative;
            z-index: 2;
            left: -50px;
        }
    }
    .img-wrapper-second{
        position: relative;
        & img:first-child{
            position: absolute;
            top: -25px;
            left: 80px;
        }
        & img:last-child{
            position: relative;
            z-index: 2;
        }
    }

    .keep-in .col{
        padding-left: 20px;
        & h2{
            margin-top: 20px;
        }
    }
    @media screen and (max-width: 991px) {
        .img-wrapper-first img:first-child {
            left: -35px;
            transform: rotate(-50deg);
        }
        .img-wrapper-second img:first-child {
            position: absolute;
            top: -25px;
            left: -40px;
            transform: rotate(40deg);
        }
        .about .col{
            flex: auto;
        }
        .easy-messag {
            margin-bottom: 30px;
            & .col{
                padding-left: 0;
            }
        }
        .keep-in .col{
            padding-left: 0;
        }
    }

    @media screen and (min-width:280px) and (max-width: 680px){
        section.about{
            padding:50px;
        }
        .img-wrapper-first{
            & img:first-child{
                display: none;
            }
            & img:last-child{
                width: 70%;
                height: 70%;
            }
        }

        .img-wrapper-second{
            & img:first-child{
                display: none;
            }
            & img:last-child{
                width: 70%;
                height: 70%;
            }
        }
    }
</style>
