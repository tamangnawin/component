<template>
  <footer>
    <p>{{ copyright }}</p>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      copyright: 'Copyright 2018 @Doersbase Softudio'
    }
  }
}
</script>

<style scoped>
    footer{
        background-color: gray;
        padding: 6px;
    }

    p{
        color: white;
        text-align: center;
    }
</style>