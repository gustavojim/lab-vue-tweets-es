<template>

    <span class='timeStamp'>
    {{props.timestamp}}    
    </span>
    
    </template>
    
    <script setup>
    import { defineProps } from 'vue';
    const props = defineProps(['timestamp']);
    </script>
    
    <style scope>
    </style>