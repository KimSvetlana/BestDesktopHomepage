<template>
    <div class='works-item'>
        <h3>{{itemHeader}}</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod.</p>
    </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

    @Component
export default class WorksItem extends Vue {
        @Prop() private itemHeader!: string;
}
</script>
