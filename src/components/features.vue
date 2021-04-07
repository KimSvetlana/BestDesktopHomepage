<template>
    <section class="features-comp" id="features-comp">
        <div class ='container'>
            <div class="row paddingRow">
                <div class='col-sm'>
                    <div class='features-item'>
                        <img src='../assets/images/Icon1.png' class='item-img' />
                        <h3 class='bannerH3'>Analysis</h3>
                        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore</p>
                    </div>
                </div>
                <div class="col-sm">
                    <div class='features-item shift'>
                        <img src='../assets/images/Icon2.png' class='item-img' />
                        <h3 class='bannerH3'>Clean Design</h3>
                        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore</p>
                    </div>
                </div>
                <div class="col-sm">
                    <div class='features-item'>
                        <img src='../assets/images/Icon3.png' class='item-img' />
                        <h3 class='bannerH3'>Messaging</h3>
                        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'

@Component({
  components: {
  }
})
export default class FeaturesComp extends Vue {}
</script>

<style lang="scss">
    @import '../assets/variables.scss';
    .features-comp {
        padding-top:165px;
        padding-bottom: 180px;
        background-color: $lightBackgroundColor ;
    }

    .features-item{
        box-sizing: border-box;
        margin: 0 auto;
        padding: 40px 14px;
        width: 362px;
        height: 290px;
        background: #FFFFFF;
        box-shadow: 0px 4px 16px rgba(0, 66, 148, 0.08);
        border-radius: 5px;

        & img{
            margin-bottom: 25px;
        }

        & h3{
            margin-bottom: 25px;
        }
        & p{
            line-height: 20px;
        }
        &.shift{
            position: relative;
            top: 50px;
        }
    }

    @media screen and (max-width: 1399px) {
        .features-item{
            width: auto;
            height: auto;
        }
    }
      @media screen and (max-width: 921px) {
       .features-comp {
            padding: 50px;
        }
        .features-comp .col-sm {
            flex: auto;
        }
        .features-item{
            margin-top:50px;
            &.shift{
                top: 0;
            }
        }
    }
</style>
