<template>
  <div class="app">
    <ChessBoard />
    <ChessSquare />
  </div>
</template>

<script>
import ChessBoard from './components/ChessBoard.vue';
import ChessSquare from './components/ChessSquare.vue';

export default {
  components: {
    ChessBoard,
    ChessSquare
  },
};
</script>

<style>
.app {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
</style>
