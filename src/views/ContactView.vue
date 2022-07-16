<script setup>
import { useCounterStore } from "@/stores/CounterStore";

let counter = useCounterStore();
</script>
<template>
  <div class="contact">
    <h1>This is a Contact page</h1>
    The current count is: {{ counter.count }}
  </div>
</template>
