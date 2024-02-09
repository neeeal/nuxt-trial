<template>
        <!-- Hero Section -->
        <Banner />

        <Section>
            <div class="p-[4rem] pt-[3rem]">

                <h2 class="font-semibold text-blue-800 text-lg">Popular Articles this Month</h2>

                <div class="flex pt-[2rem]">

                    <CardArticle/>
                    <CardArticle/>
                    <div class="border-2 rounded p-[1rem] pb-0 ml-[4rem] text-sm">
                        <h3 class="font-bold pb-[1.10rem]">Most Downloaded Articles</h3>
                        <ul class="flex flex-col justify-between text-blue-900 font-semibold  ">
                            <li v-for="popular in populars" class="flex pb-[1rem]">
                                <div class="flex-grow-2">
                                    <label>{{popular.title}}</label>
                                </div>
                                <div class="flex-grow flex-col px-[0.5rem] pt-[1rem]">
                                    <label class="flex justify-center -mb-[0.5rem] ">{{popular.views}}</label>
                                    <label class="flex text-[8px]  justify-center text-slate-600 opacity-50">VIEWS</label>
                                </div>
                                <div class="flex-grow flex-col px-[2.25rem] pt-[1rem]">
                                    <label class="flex justify-center -mb-[0.5rem]">{{popular.downloads}}</label>
                                    <label class="flex text-[8px] justify-center text-slate-600 opacity-50">DOWNLOADS</label>
                                </div>
                            </li>
                        </ul>


                    </div>

                </div>

            </div>
        </Section>

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

const populars = [
    {
        title:"Blockchain Beyond Cryptocurrency: Transforming Industries with Distributed Ledger Technology...",
        views:"10.2k",
        downloads:"48k"
    },
    {
        title:"Blockchain Beyond Cryptocurrency: Transforming Industries with Distributed Ledger Technology...",
        views:"10.2k",
        downloads:"48k"
    },
    {
        title:"Blockchain Beyond Cryptocurrency: Transforming Industries with Distributed Ledger Technology...",
        views:"10.2k",
        downloads:"48k"
    },
]
</script>