<script setup lang="ts">
import { ref, reactive } from 'vue';

import Calcurator from './calcurator/index.vue';

defineProps<{ msg: string }>();

const msg2 = ref('empty message');

const obj1 = {
    name: 'John Doe',
    age: 30,
    address: '123 Main St, Anytown, USA',
};
const obj2 = reactive({
    name: 'John Doe2',
    age: 302,
    address: '123 Main St, Anytown, USA',
});
</script>

<template>
    <h1>{{ msg }}</h1>

    <div>{{ msg2 }}</div>
    <div><input type="text" v-model="msg2" /></div>
    <div>{{ obj1.name }}</div>
    <div><input type="text" v-model="obj1.name" /></div>
    <div>{{ obj2.name }}</div>
    <div><input type="text" v-model="obj2.name" /></div>

    <Calcurator />
</template>

<style scoped>
.read-the-docs {
    color: #888;
}
</style>
