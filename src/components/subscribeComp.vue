<template>
    <section  class='subscribe'>
        <div class='container'>
            <h1 class='logo bannerH1'>AppSon</h1>
            <div class="input-group mb-3 justify-content-center">
                <input type="text" class="form-control" placeholder="Enter your Email" aria-label="Subscribe" aria-describedby="button-addon2">
                <button class="btn btn-outline-secondary btn-subscribe" type="button" id="button-addon2">Subscribe</button>
            </div>
      </div>
    </section>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
@Component({
  components: {}

})
export default class SubscribeComp extends Vue {}
</script>

<style lang="scss">
    @import '../assets/variables.scss';

    section.subscribe{
        padding-top: 119px;
        padding-bottom: 100px;
        background-color: $backgroundButtonColor;
    }
    .logo.bannerH1{
        color:white;
        margin-bottom: 27px;
    }
    .subscribe input {
        max-width: 392px;
        height: 50px;
        background-color: $darkBackgroundColor;
        border:none;
        border-radius: 25px 0 0 25px;
    }
    .subscribe input::placeholder{
        color:white;
    }
    .subscribe .btn-subscribe{
        width: 166px;
        height: 50px;
        color:$darkBackgroundColor;
        text-transform: uppercase;
        font-weight: bold;
        background-color: white;
        color:$darkBackgroundColor;
        border:none;
        border-radius: 0 25px 25px 0;

        &:hover{
            background-color: $darkBackgroundColor;
        }
    }
    @media screen and (min-width:280px) and (max-width: 680px){
       .subscribe .input-group input{
            width:100%;
            border-top-right-radius: 25px !important;
           border-bottom-right-radius: 25px !important;
        }
       .subscribe .input-group > button.btn-subscribe{
           margin-top: 20px;
           border-top-left-radius: 25px !important;
           border-bottom-left-radius: 25px !important;
       }
    }
</style>
