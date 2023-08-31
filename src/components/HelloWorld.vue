<script>
export default {
  data() {
    return {
      message: "I love Vue!",
    };
  },
  methods: {
    clearMessage() {
      this.message = "";
    },
  },
};
</script>

<template>
  <v-container class="pa-5 d-flex flex-column align-center">
    <input class="mb-5" v-model="message" />
    <v-btn class="d-inline mb-5" @click="clearMessage()">Clear</v-btn>
    <!-- <button class="d-inline" @click="message = ''">Clear</button> -->
    <h5>{{ message }}</h5>
  </v-container>
</template>

<style></style>
