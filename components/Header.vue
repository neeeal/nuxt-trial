
import type Input from 'postcss/lib/input';
<template>
    <div class="flex flex-col border border-10 border-black min-h-[10vh]">
        <div class="flex flex-1 max-h-[30rem] min-h-[4rem]">
            QCU Logo
        </div>
        <div class="flex bt-4 border-t-2 border-orange-500 bg-[#0858A4] justify-between max-h-[10rem] py-2">
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
                <div class="flex flex-grow-2 min-h-full"><Input placeholder="Search" class="justify-end italic pl-4 rounded-sm -mr-0.5"/>
                <button><img src='/assets/magnifying-glass.png' class="max-h-6 max-w-6 p-1.5 bg-[#F5F5F5] rounded-sm"/></button>
                </div>
                <div class="flex max-w-fit px-4"><Icon icon="mdi:bell" width="0.75rem" height="0.75rem" /></div>
                <div class="flex max-w-fit "><img src='/assets/heart.png' class="max-w-4 max-h-4 "/><span class="text-xs px-1">48</span></div>
                <div class="flex max-w-fit pl-12 pr-4 "><img src='/assets/user.png' class="max-w-4 max-h-4"/></div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { Icon } from '@iconify/vue';
</script>