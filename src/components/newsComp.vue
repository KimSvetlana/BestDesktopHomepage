<template>
    <section class='container news-comp'>
        <h2 class='bannerH2'>Latest News From Us</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore<br>
         et dolore magna aliqua. Lorem ipsum dolor sit amet.</p>
        <div class='row'>
            <div class="col text-start">
                <img src='../assets/images/image6.png'/>
                <h3 class="news-title">The master bedroom suite is phenomenally spacious</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
                <a href="" class='news-link'>Continue Reading <img src="../assets/images/ArrowLeft2.svg" alt=""></a>
            </div>
            <div class="col">
                <div class='news-card'>
                    <img src="../assets/images/image9.png" alt="">
                    <h3 class='new-card-title'>The master bedroom suite is phenomeny spacious</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod.</p>
                </div>
                <div class='news-card' >
                    <img src="../assets/images/image7.png" alt="">
                    <h3 class='new-card-title'>The master bedroom suite is phenomeny spacious</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod.</p>
                </div>
                <div class='news-card'>
                    <img src="../assets/images/image8.png" alt="">
                    <h3 class='new-card-title'>The master bedroom suite is phenomeny spacious</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod.</p></div>
            </div>

        </div>
    </section>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component({
  components: {}

})
export default class NewsComp extends Vue {}
</script>

<style lang="scss">
    @import '../assets/variables.scss';
    section.news-comp{
        padding-top: 130px;
    }
    .news-comp h2{
        font-weight: bold;
    }
    .news-link{
        color:$darkBackgroundColor;
        text-decoration: none;
        font-weight: bold;
        &:hover{
            text-decoration: underline;
        }
    }
    .new-card-title{
        font-size: 18px;
        font-weight: 500;
        line-height: 27px;
    }
    .news-card{
        position: relative;
        padding-left: 200px;

        & img{
            position: absolute;
            top:0;
            left:0;
        }
    }
</style>
