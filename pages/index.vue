<template>
        <!-- Hero Section -->
        <Banner />

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