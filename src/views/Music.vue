<template>
  <div id="app">
    <Tabs>
      <Tab  v-bind:key="item.id" v-for="item in music" :name="item.catégorie" :selected="item.catégorie == 'Classique'">
        <ul v-bind:key="data.title" v-for="data in item.music" >
          <img :src=data.image
          height="240px"
          width="300px">
          <li>{{data.title}}</li>
          <li>{{data.auteur}}</li>
          <li>{{data.length}}</li>
          <router-link to="/music/description">Détails</router-link>
        </ul>
      </Tab>
    </Tabs>
  </div>
</template>

<script>
  import Tab from '@/components/Tab'
  import Tabs from '@/components/Tabs'
  import json from '@/data/musics.json'

  export default {
    name: 'App',
    music: json,
    components: {
      Tab,
      Tabs,
    },
     data() {
      return {
      music: json,   
       };
  }
}
</script>

<style lang="scss">
  body {
    background-color: #bdbdbd;
    color: #fefefe;
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    font-size: 2rem;  
  }

  th, td {
    padding: 5px;
    border: 1px solid #fefefe;
    text-align: center;
  }
</style>


