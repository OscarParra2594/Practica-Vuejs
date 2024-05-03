<script setup>
import { ref } from 'vue'

let counter = ref(5)

function add() {
    counter.value++
    console.log(counter)
}
</script>

<template>
    <div @click="add" class="text-white hover:cursor-pointer bg-blue-500 rounded py-1 px-2 max-w-44 text-center select-none">
        Número de clicks: {{ counter }}
    </div>
</template>