<script setup>
import { useFlash } from "@/composables/useFlash";
let { flash } = useFlash();
</script>

<template>
  <div>
    <h1>This is an about page</h1>
    <p>
      <button
        @click="flash('Clockity', 'You have clocked from the About Page')"
      >
        Click Me
      </button>
    </p>
  </div>
</template>
