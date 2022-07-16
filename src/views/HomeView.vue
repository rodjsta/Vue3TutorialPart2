<script setup>
import TabbableTextarea from "@/components/TabbableTextarea.vue";
import { ref } from "vue";
import { state } from "@/stores/quizStore";

let comment = ref("test value");

setTimeout(() => {
  comment.value = "rod rocks the\n\nworlds";
}, 2000);
</script>

<template>
  <main>
    <form>
      <TabbableTextarea v-model="comment" style="width: 100%; height: 300px" />
    </form>
  </main>
</template>
