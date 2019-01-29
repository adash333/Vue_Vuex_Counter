<template>
  <div id="app">
    <v-app id="inspire">
      <v-toolbar color="indigo" dark fixed app>
        <v-toolbar-title>Vue Vuex Counter</v-toolbar-title>
      </v-toolbar>

      <v-content>
        <v-container fluid fill-height> <counter></counter> </v-container>
      </v-content>
    </v-app>
  </div>
</template>

<script>
import Counter from "./components/Counter";

export default {
  data() {
    return {};
  },
  components: {
    Counter
  }
};
</script>
