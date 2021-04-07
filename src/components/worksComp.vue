<template>
    <section class='works-comp'>
        <div class='container'>
            <h2 class="bannerH2">How Does It Works?</h2>
            <p class="text">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore<br>
                et dolore magna aliqua. Lorem ipsum dolor sit amet.</p>
            <div class='row paddingRow'>
            <div class="col works-item">
                <img src="../assets/images/Icon4.png" alt="">
                <h3 class="bannerH3">Create An Account</h3>
                <p>Lorem ipsum dolor sit amet, consectetur<br> adipisicing elit, sed do eiusmod.</p>
            </div>
            <div class="col works-item">
                <img src="../assets/images/Icon5.png" alt="">
                <h3 class="bannerH3">Confirm Email</h3>
                <p>Lorem ipsum dolor sit amet, consectetur<br> adipisicing elit, sed do eiusmod.</p>
            </div>
            <div class="col works-item">
                <img src="../assets/images/Icon6.png" alt="">
                <h3 class="bannerH3">See Results</h3>
                <p>Lorem ipsum dolor sit amet, consectetur<br> adipisicing elit, sed do eiusmod.</p>
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
export default class WorksComp extends Vue {}
</script>

<style lang="scss">
    @import '../assets/variables.scss';

    section.works-comp{
        background-color: $lightBackgroundColor;
        padding-top: 122px;
        padding-bottom: 120px;
    }
    .works-comp h2{
        margin-bottom: 25px;
    }
    .works-comp .text{
        margin-bottom: 45px;
    }
    .works-comp h3{
        margin-top: 30px;
        margin-bottom: 20px;
    }
    .works-comp .row{
        background: url("../assets/images/Line.png") top 50px left 50% no-repeat;
    }
    @media screen and (max-width: 1199px) {
        .works-comp .row{
            background: none;
        }
    }
    @media screen and (max-width: 921px) {
        .works-comp .col {
            flex: auto;
        }
    }
</style>
