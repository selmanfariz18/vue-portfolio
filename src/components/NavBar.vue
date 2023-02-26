<template>
    <v-app-bar app color="black" dark>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
      <v-icon color="red" left class="mr-2">fas fa-signature</v-icon>
      <v-toolbar-title color="red">Selman</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text @click="scroll('home')" class="text-red">Home</v-btn>
      <v-btn text @click="scroll('about')">About</v-btn>
      <v-btn text @click="scroll('Projects')">Projects</v-btn>
      <v-btn text @click="scroll('skills')">Skills</v-btn>
      <v-btn text @click="scroll('contact')">Contact</v-btn>
    </v-app-bar>

    <v-navigation-drawer app v-model="drawer">
      <v-list>
        <v-list-item v-for="(item, index) in items" :key="index" @click="drawer = false">
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
</template>

<script>
export default {
    methods:{
        scroll(refName){
            const element=document.getElementById(refName);
            element.scrollIntoView({behavior:"smooth"});
        }
    }, 
  data() {
    return {
      drawer: false,
      items: [
        { title: 'Home' },
        { title: 'About' },
        { title: 'Projects' },
        { title: 'skills'},
        { title: 'Contact'},
      ],
    };
  },
};
</script>

<style>

</style>