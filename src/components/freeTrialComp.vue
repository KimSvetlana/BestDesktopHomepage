<template>
     <section class='free-trial'>
        <div class="container">
          <div class='row paddingRow'>
            <div class= "col text-start">
              <h2 class="bannerH2">Try 30 Days Free Trial</h2>
              <p>No credit card reauired</p>
            </div>
            <div class= "col align-self-center">
              <button class="btn free-trial-btn">Get Stared
                <img src="../assets/images/ArrowLeft.svg"/>
              </button>
            </div>
          </div>
       </div>
    </section>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component({
  components: {}
})
export default class FreeTrialComp extends Vue {}
</script>

<style lang="scss">
 @import '../assets/variables.scss';

  section.free-trial{
    padding-top: 135px;
    padding-bottom: 100px;
    background-color: $lightBackgroundColor;
  }
  .free-trial .col:first-child{
    padding-left: 220px;
  }
  .free-trial .col:last-child{
    padding-right: 150px;
  }
  .free-trial h2{
    font-weight: bold;
    margin-bottom: 25px;
  }
  button.free-trial-btn{
    box-sizing: border-box;
    padding: 14px 68px;
    color:white;
    font-weight: bold;
    border-radius: 25px;
    background-color: $backgroundButtonColor;
    &:hover{
      background: none;
      border: 2px solid  $backgroundButtonColor;
      color: $backgroundButtonColor;
    }
  }
   @media (max-width: 1199px){
      .free-trial .col:first-child{
        padding-left: 20px;
      }
    .free-trial .col:last-child{
      padding-right: 20px;
    }
   }
    @media screen and (min-width:280px) and (max-width: 680px){
      .free-trial .col{
        flex:auto;
        text-align: center !important;
      }
    }
</style>
