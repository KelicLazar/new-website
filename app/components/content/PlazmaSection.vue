<script setup>
defineProps({
  plazmaTitle: { type: String, required: true },
  plazmaDescription: { type: String, default: "" },
});
</script>

<template>
  <section class="blabla" :style="{ backgroundColor }">
    <div class="container">
      <h1>plazmaTitleplazmaTitleplazmaTitle plazmaTitle plazmaTitle</h1>
      <h1>{{ plazmaTitle }}</h1>
      <p>{{ plazmaTitle }}</p>
    </div>
  </section>
</template>
