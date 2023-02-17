<template>
  <v-app id="home">
    <NavBar/>
    <v-container fluid>
      
    </v-container>
  </v-app>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue'

export default {
  name: 'HomeView',
  components: {
    NavBar
  }
}
</script>
