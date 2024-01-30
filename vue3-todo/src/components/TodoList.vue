<template>
    <ul>
        <li v-for="(item, index) in todoItems" :key="index">{{ item }}</li>
    </ul>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps(['todoItems']);

</script>

<style lang="scss" scoped></style>
