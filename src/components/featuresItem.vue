<template>
    <div class='features-item'>
        <h3>{{itemHeader}}</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore</p>
    </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

    @Component
export default class FeaturesItem extends Vue {
        @Prop() private itemHeader!: string;
        @Prop() private itemText!:string;
        @Prop() private imgSrc!:string;
}
</script>
