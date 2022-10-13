<template>
  <img src="props.src" class="profile" alt="Profile Image" tweet=""/>
</template>

<script>
import { defineProps } from 'vue';
const props = defineProps(['src']);
</script>


<style scoped>
</style>