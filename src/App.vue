<template>
  <div id="app">
    <Main/>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import Main from './components/main.vue'
@Component({
  components: {
    Main
  }

})
export default class App extends Vue {}
</script>

<style lang="scss">
  @import 'assets/variables.scss';
  @import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@300;400;500;700&display=swap');
#app {
  font-family: 'Quicksand', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  font-weight: 300;
  font-size: 16px;
  line-height: 20px;
  color: #000000;
}
</style>
