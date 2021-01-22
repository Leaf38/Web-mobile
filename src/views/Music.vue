<template>
  <div id="app">
    <Tabs>
      <Tab name="Classique" selected="true">
        <ul>
          <li>Classique 2</li>
          <li>Classique 3</li>
          <li>Classique 4</li>
          <li>Classique 5</li>
        </ul>
      </Tab>
      <Tab name="Jazz">
        <ul>
          <li>Jazz 1</li>
          <li>Jazz 2</li>
          <li>Jazz 3</li>
          <li>Jazz 4</li>
          <li>Jazz 5</li>
        </ul>
      </Tab>
      <Tab name="Variété">
        <ul>
          <li>Variété 1</li>
          <li>Variété 2</li>
          <li>Variété 3</li>
          <li>Variété 4</li>
          <li>Variété 5</li>
        </ul>
      </Tab>
    </Tabs>
  </div>
</template>

<script>
  import Tab from '@/components/Tab'
  import Tabs from '@/components/Tabs'

  export default {
    name: 'App',
    components: {
      Tab,
      Tabs
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


