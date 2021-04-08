<template>
    <header class="header-comp" id="header-comp">
        <b-navbar toggleable="lg" variant="info" class="container">
            <b-navbar-brand href="#">AppSon</b-navbar-brand>
            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav>
                    <b-nav-item href="#" class="active">Home</b-nav-item>
                    <b-nav-item href="#">Feature</b-nav-item>
                    <b-nav-item href="#">Pricing</b-nav-item>
                    <b-nav-item href="#">Pages</b-nav-item>
                </b-navbar-nav>
                <button class="btn nav-btn">Sign up</button>
            </b-collapse>
        </b-navbar>
        <section class="header-content container">
            <div class="row">
                <div class="col">
                    <h1 class='header-title bannerH1'>Best Desktop App for You</h1>
                    <p class='header-text'>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor<br>
                    incididunt ut labore et dolore magna aliqua. adipisicing elit, sed do eiusmod tempor <br>
                    incididunt ut labore et dolore magna aliqua.</p>
                    <button class='btn btn-download'>Download</button>
                    <button  class='btn btn-trial'>Free Trial</button>
                    <div class='phones'></div>
                    <a class="header-scrol-down" href="#footer"><img src='../assets/images/ScrolDown.png'/></a>
                </div>
            </div>
        </section>
    </header>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'

@Component({
  components: {
  }
})
export default class HeaderComp extends Vue {}
</script>

<style lang="scss">
    @import '../assets/variables.scss';
    header{
        background: url('../assets/images/headerBackground.png') no-repeat;
        background-position: top 0px left 0px;
        box-shadow: -7px -7px 32px rgba(0, 30, 67, 0.06);
        background-size: cover;
    }
    header .navbar{
        padding: 0;
        &.bg-info{
            background-color: rgba(0, 0, 0, 0) !important;
        }
    }

    header .navbar .navbar-brand{
        display: block;
        width: 179px;
        height: 100px;
        padding-top: 25px;
        color: white;
        background-color: $backgroundButtonColor;
        border-radius: 0px 0px 21.5px 21.5px;
        font-weight: bold;
        font-size: 36px;
        line-height: 45px;
    }

    .navbar-nav .nav-item {
        margin-left: 25px;
        font-weight: 500;
        text-transform: uppercase;
        color: rgba(0, 0, 0, 0.55);
    }

    ul.navbar-nav .nav-item .nav-link:hover{
        text-decoration: underline;
    }
    .navbar-nav .nav-item.active .nav-link{
        color: #0F7CFF;
    }

    ul.navbar-nav {
        margin-left: auto;
    }
    .navbar .nav-btn{
        box-sizing: border-box;
        width: 165px;
        height: 50px;
        margin-left: 52px;
        text-transform: uppercase;
        font-weight: 700;
        color: white;
        background: $darkBackgroundColor;
        border-radius: 25px;
        &:hover{
            border: 2px solid $darkBackgroundColor;
            background: none;
        }
    }

    .header-content{
        position: relative;
        padding-top: 88px;
    }
    .header-text{
        margin-top: 30px;
        margin-bottom: 33px;
        font-weight: 400;
        line-height: 169%;
        color: #929292;
    }
    header .btn-download,
    header .btn-trial{
        box-sizing: border-box;
        font-weight: 700;
        width:166px;
        height: 50px;
        border-radius: 25px;
        margin-bottom: 108px;
    }
    header .btn-download{
        color:white;
        margin-right: 30px;
        background-color: $backgroundButtonColor;
        &:hover{
            color:$backgroundButtonColor;
            background-color: white;
            border: 2px solid $backgroundButtonColor;
        }
    }
    header .btn-trial{
        color:$backgroundButtonColor;
        border:2px solid $backgroundButtonColor;
        &:hover{
            color: white;
            background-color:  $backgroundButtonColor;
        }
    }

    div.phones{
        margin:0 auto;
        overflow: hidden;
        width: 798px;
        height: 494px;
        background: url('../assets/images/Phone2.png') top -40px left 50% no-repeat,
         url('../assets/images/Phone1.png') top 50px left -10% no-repeat,
         url('../assets/images/Phone3.png') top 50px left 105% no-repeat;
    }

    .header-scrol-down{
        position: absolute;
        bottom: -55px;
        left: 46.5%;
    }
    @media screen and (max-width: 921px) {
        div.phones{
            width: 312px;
            background: url('../assets/images/Phone2.png') top -40px left 50% no-repeat,
        }
         .header-scrol-down{
            left: 42.5%;
        }
    }
    @media screen and (max-width: 385px){
        header .btn-download {
            margin-right: 0px;
        }
        header .btn-download,
        header .btn-trial{
            margin-bottom: 20px;
        }
    }
    @media screen and (min-width: 375px) and (max-width:1919px){
        header{
            background: url('../assets/images/headerBackground.png') no-repeat;
            background-position: top 25px left 0px;
        }
    }
</style>
