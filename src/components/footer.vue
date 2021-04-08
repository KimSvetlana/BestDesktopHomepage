<template>
    <footer id='footer'>
        <div class="container">
            <div class='row paddingRow'>
                <div class='col-4 copiraight'>
                <p>© 2018 Copyright, All Rights Reserved by AppSon</p>
                </div>
                <div class='col'>
                    <nav class="nav justify-content-end">
                        <a class="nav-link" href="#">Terms & Condition</a>
                        <a class="nav-link" href="#"> PrivacyPolicy</a>
                        <a class="nav-link" href="#"> Help</a>
                    </nav>
                </div>
                <div class='col-2'>
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
                <a class='footer-scrol-up' href="#header-comp"><img src="../assets/images/ScrollUp.png"></a>
                </div>
            </div>
        </div>
    </footer>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
@Component({
  components: {}

})
export default class Footer extends Vue {}
</script>

<style lang="scss">
    @import '../assets/variables.scss';

    footer {
        position: relative;
        padding-top: 50px;
        padding-bottom: 30px;
        background-color: $darkBackgroundColor;
        & p{
            color:white;
        }
    }
    footer .nav-link{
        color:white;
        &:hover{
            display: inline-flex;
            text-decoration: underline;
            color: white;
        }
    }
    .footer-social-list{
        list-style: none;
        float: right;
        & li{
            display: inline-block;
            margin-left: 15px;
        }
    }
    .footer-scrol-up{
        position: absolute;
        right: 8.2%;
        bottom: 18%;
    }

     @media screen and (max-width: 1700px) {
         .footer-scrol-up{
             right: 1.2%;
        }

     }
     @media screen and (max-width: 1495px) {
         footer .nav{
             display: list-item;
            justify-content: center !important;
        }
        .footer-social-list{
            float:left;
            & li{
                display: list-item;
           }
        }
     }
    @media screen and (max-width: 730px) {
        footer .col {
            flex: auto;
            }
        footer .col-4 {
            width: 100%;
        }
        footer .col-2 {
            width: 100%;
        }
        .footer-social-list{
            padding:0;
            float:none;
            margin-top: 10px;
            & li{
                display: inline-block;
           }
        }
    }
</style>
