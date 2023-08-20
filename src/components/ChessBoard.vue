<template>
  <div class="chess-board">
    <div v-for="(row, rowIndex) in board" :key="rowIndex" class="chess-row">
      <ChessSquare
        v-for="(square, colIndex) in row"
        :key="colIndex"
        :piece="square.piece"
        @click="handleSquareClick(rowIndex, colIndex)"
      />
    </div>
  </div>
</template>

<script>
import ChessSquare from './ChessSquare.vue';

export default {
  components: {
    ChessSquare,
  },
  // ...
};
</script>
