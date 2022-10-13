<template>

    <span class='user'>
<!-- LLamar a los datos de la matriz en app.vue -->
        <span class="name">{{props.users}}</span>
        <span class="span">{{props.handle}}</span>
    </span>
    
    </template>
    
    <script setup>
    import { defineProps } from 'vue';
    const props = defineProps(['users','handle']);
    </script>
    
    <style scope>
    </style>