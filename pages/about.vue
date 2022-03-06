<template>
  <main>about on {{ rendered }}</main>
</template>

<script>
export default {
  asyncData() {
    let rendered = process.server ? "server" : "client";
    return {
      rendered,
    };
  },
};
</script>

<style>
</style>