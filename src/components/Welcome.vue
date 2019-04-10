<template>
  <v-container>
    <v-layout
      text-xs-center
      wrap
    >
      <v-flex xs12>
        <v-img
          :src="require('../assets/comp_website.jpeg')"
          contain
          height="200"
        ></v-img>
      </v-flex>
      <v-flex mb-4>
        <h1 class="display-2 font-weight-bold mb-3">
          <br> Hi! I'm Lachlan. <br>
          Welcome to my website
        </h1>
        <p class="subheading font-weight-regular">
          📖 Monash University - Computer Science Student<br>
          💰 National Australia Bank - Intern Software Engineer<br>
          💻 AI Media - Software Developer<br>
        </p>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
      links: {
        "link": "https://github.com/etopiei",
        "title": "GitHub"
      }
    })
  }
</script>

<style>
</style>
