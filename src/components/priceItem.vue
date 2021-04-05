<template>
    <div class='works-item'>
        <h3>{{priceHeader}}</h3>
        <p>2gb Hosting<br>
            10 Custom Domain<br>
            SSD Hosting<br>
            50 gb Bandwith<br>
            Free Support<br>
        </p>
        <p class="item-cost">${{itemCost}}</p>
        <button class='btn'>Try Now</button>
    </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

    @Component
export default class PriceItem extends Vue {
        @Prop() private priceHeader!: string;
        @Prop() private itemCost!: string;
}
</script>
