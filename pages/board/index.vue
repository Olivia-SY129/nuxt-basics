<template lang="">
  <div>
    <h3>Board</h3>
    <MainButton />
  </div>
</template>
<script>
export default {
  methods: {
    movePage() {
      this.$router.push({
        name: "board",
        params: {
          board: "board",
        },
      });
    },
  },
};
</script>
<style lang=""></style>
