<template>
    <section class="container price">
        <div class='row paddingRow'>
            <div class="col price-title text-start">
                <h2 class='bannerH2'>Pricing Plan</h2>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet.</p>
                <button class='btn monthly'>Monthly</button>
                <button class='btn yearly'>Yearly</button>
            </div>
            <div class="col">
                <div class='price-item premium'>
                    <img src="../assets/images/Icon7.png" alt="">
                    <h3 class="bannerH3">Premium</h3>
                    <hr/>
                    <p>2gb Hosting<br>
                        10 Custom Domain<br>
                        SSD Hosting<br>
                        50 gb Bandwith<br>
                        Free Support<br>
                    </p>
                    <p class="item-cost">$49.00</p>
                    <button class='btn'>Try Now</button>
                </div>
            </div>

            <div class="col">
                <div class='price-item standart'>
                    <img src="../assets/images/Icon8.png" alt="">
                    <h3 class="bannerH3">Standart</h3>
                    <hr/>
                    <p>2gb Hosting<br>
                        10 Custom Domain<br>
                        SSD Hosting<br>
                        50 gb Bandwith<br>
                        Free Support<br>
                    </p>
                    <p class="item-cost">$19.00</p>
                    <button class='btn'>Try Now</button>
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
export default class PriceComp extends Vue {}
</script>

<style lang="scss">
@import '../assets/variables.scss';
    section.price{
        padding: 130px 0;
    }
    .col.price-title{
        margin: auto;
        padding-left: 30px;
        margin-right: 35px;
        & h2{
            margin-bottom: 30px;
        }
        & p{
            margin-bottom: 40px;
            line-height: 24px;
        }
    }
    .price-item{
        box-sizing: border-box;
        width: 362px;
        height: 576px;
        padding: 39px 30px;
        background: #FFFFFF;
        box-shadow: 0px 4px 20px rgba(0, 36, 80, 0.08);
        border-radius: 5px;

        & img{
            margin-bottom: 20px;
        }
        & h3{
            margin-bottom: 25px;
        }
        & p{
            line-height: 29px;
            margin-bottom: 40px;
        }

        & hr{
            margin-bottom: 23px;
        }
        & .item-cost {
            color:$backgroundButtonColor;
            font-weight: 500;
            font-size: 32px;
            line-height: 22px;
            margin-bottom: 30px;
        }
    }
    .premium button{
        box-sizing: border-box;
        width: 166px;
        height: 50px;
        color:white;
        background: $backgroundButtonColor;
        border-radius: 25px;
        &:hover{
            color:$backgroundButtonColor;
            background-color: white;
            border:2px solid $backgroundButtonColor;
        }
    }

    .standart button{
        box-sizing: border-box;
        width: 166px;
        height: 50px;
        color:$backgroundButtonColor;
        border:2px solid $backgroundButtonColor;
        border-radius: 25px;
        &:hover{
            color:white;
            background: $backgroundButtonColor;
        }
    }
    button.monthly{
        box-sizing: border-box;
        width: 166px;
        height: 50px;
        color:white;
        background: $backgroundButtonColor;
        border-radius: 25px 0 0 25px;
        &:hover{
            color:$backgroundButtonColor;
            background-color: $lifhtButtonColor;
            border:3px solid $backgroundButtonColor;
        }
    }

    button.yearly{
        box-sizing: border-box;
        width: 166px;
        height: 50px;
        color:$backgroundButtonColor;
        border:3px solid $backgroundButtonColor;
        border-radius: 0 25px 25px 0;
        &:hover{
            color:white;
            background: $lifhtButtonColor;
        }
    }
    .col .standart{
        margin-right: 20px;
    }
    @media screen and (max-width: 1399px) {
        .col.price-title{
            padding-left: 0px;
            margin-right: 0px;
        }
        button.monthly,
        button.yearly{
            width:100px;
        }
        .price-item{
            width: 332px;
            height: 506px;
            padding: 20px 15px;
           & img{
                margin-bottom: 10px;
            }
            & h3{
                margin-bottom: 15px;
            }
            & p{
                margin-bottom: 20px;
            }

            & hr{
                margin-bottom: 13px;
            }
            & .item-cost {
                font-size: 20px;
                margin-bottom: 15px;
            }
        }
    }
    // @media screen and (min-width: 922px) and (max-width: 991px) {
    //     .price-item .standart{
    //         margin: 0 auto;
    //         margin-top: 30px;
    //     }
    // }
    @media screen and (max-width: 921px) {
        .price .col{
            flex: auto;
            text-align: center !important;
        }
        .col .standart{
            margin-right: auto;
        }
        .price-item{
            margin: 0 auto;
            margin-top: 20px;
        }
    }
    @media screen and (min-width: 375px) and (max-width:580px) {
        section.price {
            padding: 40px 0;
        }
        .price .price-title{
            padding: 0 15px;
        }
    }

</style>
