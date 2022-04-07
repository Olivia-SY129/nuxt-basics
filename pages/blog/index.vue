<template>
  <div>
    <div class="blog-title">블로그 메인</div>
    <Nuxt />
  </div>
</template>

<script>
export default {
  layout: "blog",
};
</script>

<style>
.blog-title {
  margin: 0 auto;
  display: flex;
  min-height: 100vh;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
