
import type Input from 'postcss/lib/input';
<template>
    <div class="flex flex-col min-h-[10vh]">
        <div class="flex flex-1 max-h-[30rem] min-h-[4rem] pt-[0.3rem] pl-[4rem]">
            <img src="/assets/qcu-logo.png" class="w-[3rem] h-[3rem]"/>
            <div class="flex flex-col  pl-[0.5rem] pt-[0.3rem]">
                <img src="/assets/qcu-text.png" class="w-[20rem] h-[2rem]"/>
                <span class="pl-[0.3rem] text-blue-900 -mt-[0.5rem] text-xl  tracking-wider ">Open Access Journal</span>
            </div>
        </div>
        <div class="flex bt-4 border-t-4 border-orange-500 bg-[#0858A4] justify-between max-h-[10rem] py-2">


            <!-- Naviigation -->
            <div class="flex flex-grow-1 max-w-full pl-16 items-center text-white text-sm">
                <div class="flex max-w-fit px-4 justify-center">Home</div>
                <div class="flex max-w-fit px-4 justify-center items-center">About
                    <Icon icon="gridicons:dropdown" width="1rem" height="1rem" />
                </div>
                <div class="flex max-w-fit px-4 justify-center items-center">QCU Journal
                    <Icon icon="gridicons:dropdown" width="1rem" height="1rem" />
                </div>
                <div class="flex max-w-fit px-4 justify-center">Announcements</div>
                <div class="flex max-w-fit px-4 justify-center">Pricing</div>
                <div class="flex max-w-fit px-4 justify-center">Guidelines</div>
                <div class="flex max-w-fit px-4 justify-center">Indexing</div>
            </div>


            <div class="flex flex-grow-0 text-white text-sm items-center max-h-[10rem]">
                <div class="flex flex-grow-2 min-h-full">
                    <Input placeholder="Search" class="justify-end italic pl-4 rounded-sm -mr-5 text-black w-full pr-6  "/>
                    <button>
                        <img src='/assets/magnifying-glass.png' class="max-h-6 max-w-6 p-1.5 bg-[#F5F5F5] rounded-sm"/>
                    </button>
                </div>
                
                    <button class=" flex max-w-fit flex-grow px-4">
                        <Icon icon="mdi:bell" width="0.75rem" height="0.75rem" /><div class="relative right-1.5 bottom-0.5 bg-red-600 border border-[#0858A4] rounded-3xl h-2 w-2 "/>
                    </button>

                <div class="flex max-w-fit "><img src='/assets/heart.png' class="max-w-4 max-h-4 "/><span class="text-xs px-1">48</span></div>
                <div class="flex max-w-fit pl-12 pr-4 "><img src='/assets/user.png' class="max-w-4 max-h-4"/></div>
            </div>

            
        </div>
    </div>
</template>

<script setup>
import { Icon } from '@iconify/vue';

const notification = 1
</script>