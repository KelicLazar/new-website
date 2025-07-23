<script setup>
// const appConfig = useAppConfig();
const route = useRoute();
// console.log(route.path, route);
const { data: val } = await useAsyncData(route.path, () =>
  queryCollection("content").path(route.path).first()
);
// This will handle all dynamic pages from your content

const nuxtApp = useNuxtApp();

if (nuxtApp.ssrContext) {
  console.log("Running on the server");
} else {
  console.log("Running on the client");
}

console.log("VAL", route.path, val.value);
// console.log(appConfig);
</script>

<template>
  <div class="bg-red-500">
    <br /><br />
    <br /><br />
    <br /><br />
    <br /><br />
    <!-- <ContentRenderer v-if="val" :value="val" /> -->
    <div>
      not working not workings not working not working not working not working
      not working not working not working
    </div>
  </div>
</template>
