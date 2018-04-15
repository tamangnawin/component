<template>
  <header>
    <h1>{{ title }}</h1>
  </header>
</template>

<script>
export default {
  data() {
    return {
      title: 'Doersbase Softudio'
    }
  }
}
</script>

<style scoped>
  header{
    background:grey;
    padding: 10px;
  }

  h1{
    color:white;
    text-align: center;
  }
</style>