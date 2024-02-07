<template>
    {{ console.log(bgColor) }}
    <button v-if="active ==='on'" class="bg-blue-900 text-white text-sm  border w-11/12 h-10 rounded-2xl mx-auto my-3.5">button</button>
</template>

<script setup>

const props = defineProps({
    active: {
        type: String
    }
    // bgColor: {
    //     type: String,
    //     default: "bg-blue-900"
    // }
})
</script>