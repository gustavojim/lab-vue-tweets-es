<template>

<p class='message'>
{{props.mensaje}}    
</p>

</template>

<script setup>
import { defineProps } from 'vue';
const props = defineProps(['mensaje']);
</script>

<style scope>
</style>