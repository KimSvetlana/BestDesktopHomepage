<template>
<div class='container-fluid'>
  <h1>{{msg}}</h1>
  <button type="button" class="btn btn-primary">Primary</button>
</div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class Main extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
