<template>
  <div>
    <app-header></app-header>
    <app-dummy></app-dummy>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Dummy from './components/Dummy.vue';
import Footer from './components/Footer.vue';
export default {
  components: {
    'app-header': Header,
    'app-dummy': Dummy,
    'app-footer': Footer
  },
  data() {
    return {

    }
  }
}
</script>

<style>

</style>
