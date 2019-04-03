<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>etopiei's website</span>
      </v-toolbar-title>
    </v-toolbar>
    <v-content>
      <Welcome/>
    </v-content>
  </v-app>
</template>

<script>
import Welcome from './components/Welcome';

export default {
  name: 'App',
  components: {
    Welcome,
  },
  data() {
    return {
      //
    };
  },
};
</script>
