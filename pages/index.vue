<template>
    <!-- Hero Section -->
    <div class="flex flex-col min-h-[40vh] bg-center bg-cover bg-no-repeat bg-[url('/assets/qcu-building.jpg')] bg-opacity-20">
    <!-- <div class="absolute bg  inset-0 bg-blue-800 opacity-70"></div> -->
    <div class="flex flex-col w-1/2 justify-center flex-grow pl-12">
        <h4 class="text-xs text-white">Quezon City University’s Directory of Journals</h4>
        <h1 class="py-2 text-2xl text-white">Find or Submit Open Access Articles</h1>
        <div class="flex flex-row">
            <button class="bg-orange-500 text-xs text-white rounded-xl border py-2 px-6 mr-4 my-2">Browse Articles</button>
            <button class="border border-white text-white text-xs rounded-xl py-2 px-6 mr-4 my-2">Be a Contributor</button>
        </div>
    </div>
</div>



    <Section> Section </Section>

    <Section> Section </Section>
    
    <Section> Section </Section>
    
    <Section> Section </Section>
    
    <!-- QOAJ Plans Section -->
    <Section>
        <h2 class="pt-4 text-2xl text-blue-800 font-semibold  text-center">QOAJ Plans</h2>
        <div class="flex flex-1 justify-between mx-auto max-w-4xl">
            <CardPlan></CardPlan>
            <CardPlan :active="active"></CardPlan>
            <CardPlan :active="active"></CardPlan>
        </div>
    </Section>

    <!-- FOOTER -->
    <div class="flex flex-col min-h-[25vh] justify-center">
        <div class="flex flex-row border">
            <div class="flex flex-1 justify-center border">
                Left
            </div>
            <div class="flex flex-1 justify-center">
                Form
            </div>
        </div>
        <div class="py-3">
            Bottom text
        </div>
    </div>
</template>

<script setup>
const active = "on"
</script>