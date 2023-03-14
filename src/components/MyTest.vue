<script setup lang="ts">
/** The top-level await causes event handling to not work (button click) */
await new Promise((resolve) => setTimeout(resolve, 1000));

function wow() {
  console.log("wow!!");
}
</script>

<template>
  <div>
    Hello!
    <button @click="wow">Go go go</button>
  </div>
</template>
