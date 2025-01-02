<script setup lang="ts">
// import { ref, reactive } from 'vue';
</script>

<template>
    <div class="numbers">
        <button>9</button>
        <button>8</button>
        <button>7</button>
        <button>6</button>
    </div>
</template>

<style scoped>
.numbers {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
}
</style>
