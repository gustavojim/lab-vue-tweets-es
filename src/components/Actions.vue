<template>

<!-- Copiando el div Actions del App.vue -->

<div class="actions"> 
    <i class="far fa-comment"></i>
    <i class="fas fa-retweet"></i>
    <i class="far fa-heart"></i>
    <i class="fas fa-share"></i>
</div>

</template>

<script setup>
import { defineProps } from 'vue';
const props = defineProps(['src']);
</script>

<style scoped>
</style>