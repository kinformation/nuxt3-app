<template>
  <div>
    count: {{ count }}
    <v-btn color="primary" @click="addCount">+</v-btn>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";

const count = ref(0);
function addCount() {
  count.value++;
}
</script>
