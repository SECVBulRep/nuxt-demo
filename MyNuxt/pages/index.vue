<template>
  <div class="Main">
    Main page
    <ContentDoc></ContentDoc>
  </div>
</template>
<script>
definePageMeta({
  middleware: "auth",
});

const { sayHello } = useUtils();
sayHello();
</script>
<style scoped></style>
