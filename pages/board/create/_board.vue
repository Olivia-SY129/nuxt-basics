<template lang="">
  <div>
    <h1>create</h1>
    <h3>{{ $route.params.board }}</h3>
    <MainButton @click="movePage" />
  </div>
</template>
<script>
export default {
  methods: {
    movePage() {
      this.$router.push({
        name: "board-create-board",
        params: {
          board: "humor",
        },
        query: {
          page: 5,
        },
      });
    },
  },
};
</script>
<style lang=""></style>
