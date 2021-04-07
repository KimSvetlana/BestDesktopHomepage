<template>
     <section class='free-trial'>
        <div class="container">
          <div class='row'>
            <div class= "col">
              <h2 class="bannerH2">Try 30 Days Free Trial</h2>
              <p>No credit card reauired</p>
            </div>
            <div class= "col">
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
    padding-top: 133px;
    padding-bottom: 113px;
    background-color: $lightBackgroundColor;
  }
  .free-trial h2{
    font-weight: bold;
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
</style>
