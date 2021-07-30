<template>
  <div class="content">
    <div class="newItem">
      <input class="itemInput" type="text" id="itemInput" placeholder="Create a New Todo..." />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      input: "",
    };
  },
};
</script>

<style scoped>
.content {
  position: relative;
  top: -15px;
}
</style>
