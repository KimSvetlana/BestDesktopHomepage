<template>
    <footer id='footer'>
        <div class="container">
            <div class='row'>
                <div class='col copiraight'>
                <p>© 2018 Copyright, All Rights Reserved by AppSon</p>
                </div>
                <div class='col'>
                    <nav class="nav justify-content-end">
                        <a class="nav-link" href="#">Terms & Condition</a>
                        <a class="nav-link" href="#"> PrivacyPolicy</a>
                        <a class="nav-link" href="#"> Help</a>
                    </nav>
                </div>
                <div class='col'>
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
        padding: 50px;
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
        & li{
            display: inline-block;
        }
    }
     @media screen and (max-width: 921px) {
        footer .col {
            flex: auto;
        }
    }
</style>
