<template>
  <div id="app">
    <SatCard/>
    <ActCard/>
    <SatCard/>
    <ActCard/>
  </div>
</template>

<script>
import SatCard from './components/SatCard.vue'
import ActCard from './components/ActCard.vue'

import axios from 'axios'

export default {
  name: 'app',
  components: {
    SatCard,
    ActCard,
  },
  data() {
      return {
          results: []
      }
  },
  mounted() {
      axios.get('http://www.mocky.io/v2/5b2aa8a43000000e009cd439').then(response => {
          console.log(response.data.courses);
          this.results = response.data.courses;
      });
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Muli:200,400,800');

#app {
  font-family: 'Muli', sans-serif;
  display: flex;
  flex-flow: row;
  justify-content: space-around;
  align-items: center;
  flex-wrap: nowrap;
}

/* 576 Media Query */
@media (max-width: 767px) {
  #app {
    flex-wrap: wrap;
  }

}

</style>
