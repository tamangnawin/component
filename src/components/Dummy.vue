<template>
  <div id="ninjas">
      <h1>The developer team of Doersbase Softudio</h1>
      <ul>
          <li v-for="ninja in ninjas" :key="ninja.id" v-on:click="ninja.show = !ninja.show">
              
              <h2>{{ ninja.name }}</h2>
              
              <h3 v-show="ninja.show">{{ ninja.expert }}</h3>
          </li>
      </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
        ninjas: [
            {name: 'Solam', expert:'Java', show:false},
            {name: 'Krishna', expert:'JavaScript', show:false},
            {name: 'Suraz', expert:'JavaScript', show:false},
            {name: 'Mahesh', expert:'PHP', show:false}
        ]
    }
  }
}
</script>

<style scoped>
    #ninjas{
    width: 100%;
    max-width: 900px;
    margin: 40px auto;
    padding: 0 20px;
    box-sizing: border-box;
    cursor: pointer;
    overflow: hidden;
}
    #ninjas h1{
        text-align: center;
    }
    ul{
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;
}
    li{
    flex-grow: 1;
    flex-basis: 300px;
    text-align: center;
    padding: 30px;
    border: 1px solid #222;
    margin: 10px;
}
</style>