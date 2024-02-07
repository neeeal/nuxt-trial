<template>
    <div class="flex flex-col justify-center border rounded-lg m-4">
        <h3 class="pt-4 text-2xl text-blue-800 font-sans  font-semibold  text-center">Title</h3>
        <h4 class="py-1 text-xs  text-blue-800 text-center">PHP 0.50 / credit</h4>
        <hr class=" w-4/5 mx-auto">
        <ul class="flex-col flex-1">
            <li v-for="item in items" class="flex row w-full p-2">
                <Icon icon="basil:check-solid" color="green" width="2em" height="2em" class="ml-10"/>
                <p class="w-full font-normal text-xs mr-11 pl-4 pt-2">{{ item.message }}</p>
            </li>
        </ul>
        <ButtonPrimary :active="active"></ButtonPrimary>
        
    </div>
</template>

<script setup>

import { Icon } from '@iconify/vue';
// const items = ref([{ message: 'Foo' }, { message: 'Bar' }])
const items = ref([
    {message : 'Proident ullamco dolor deserunt.'},
    {message : 'Aliqua ex officia Lorem sit quis officia sit.'},
    {message : 'Lorem laborum et esse mollit non.'}
])

const props = defineProps({
    active: {
        type: String
    }
})

</script>