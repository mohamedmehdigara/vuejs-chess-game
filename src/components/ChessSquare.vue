<template>
  <div
    class="chess-square"
    :class="{ 'selected': isSelected, 'valid-move': isValidMove }"
    @click="handleClick"
  >
    <!-- Image rendering code here -->
  </div>
</template>

<script>
export default {
  props: ['isSelected', 'isValidMove'],
  methods: {
    handleClick() {
      this.$emit('click');
    },
  },
};
</script>

<style scoped>
/* ... */
</style>
