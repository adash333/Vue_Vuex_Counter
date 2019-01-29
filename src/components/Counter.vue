<template>
  <v-flex xs12 sm6 offset-sm3>
    <v-card>
      <v-img
        src="https://cdn.vuetifyjs.com/images/cards/desert.jpg"
        aspect-ratio="2.75"
      ></v-img>

      <v-card-title primary-title>
        <div>
          <h3 class="headline mb-0">{{ count }}</h3>
        </div>
      </v-card-title>

      <v-card-actions>
        <v-btn v-on:click="decrement" color="error">-1</v-btn>
        <v-btn v-on:click="increment" color="primary">+1</v-btn>
      </v-card-actions>
    </v-card>
  </v-flex>
</template>

<script>
import { mapGetters, mapActions } from "vuex";

export default {
  name: "Counter",
  computed: {
    ...mapGetters({
      count: "getCount"
    })
  },
  methods: {
    ...mapActions(["increment", "decrement"])
  }
};
</script>
