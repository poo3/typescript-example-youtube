<template>
  <div>
    <h1>{{ message }}</h1>
    <h3>{{ fullName }}</h3>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

interface User {
  firstName: string;
  lastName: string;
}

export default Vue.extend({
  data() {
    return {
      message: "Hello World!!",
      firstName: "poo3",
      lastName: "fuma",
    };
  },
  computed: {
    fullName(): string {
      return this.firstName + this.lastName;
    },
  },
});
</script>

<style scoped></style>
