<template>
    <div class="relative flex min-h-screen bg-gray-50 p-4 mb-4 flex-col items-center">
        <div class="absolute -top-100 right-0 w-250 h-250 rotate-158 bg-[#F2FAFF] z-0"> </div>
        <div class="relative z-10 flex flex-col w-1/2">
            <section class="flex gap-4 py-4 mb-10">
                <div class="navbar flex w-full gap-4">
                    <div class="flex flex-1 gap-2 text-center items-center">
                        <Flower color="#00B289" :size="30"/>
                        <h1 class="font-bold font-sans text-[#00B289] text-2xl"> bonsai </h1>
                    </div>
                    <div class="flex flex-1 gap-6 justify-end items-center">
                        <div class="flex gap-2 items-end-safe">
                            <h1 class="font-sans">
                                Product
                            </h1>
                            <ChevronDown :size="18" />
                        </div>
                        <div class="flex gap-2 items-end-safe">
                            <h1 class="font-sans">
                                Templates
                            </h1>
                            <ChevronDown :size="18" />
                        </div>
                        <div class="flex">
                            <h1 class="font-sans">
                                Pricing
                            </h1>
                        </div>
                        <div class="flex">
                            <h1 class="font-sans">
                                Reviews
                            </h1>
                        </div>
                    </div>
                    <div class="flex flex-1 justify-center gap-4">
                        <button class="w-20 h-10 border-2 border-[#00B289] rounded-md text-center">
                            <span class="font-bold font-sans text-[#00B289] text-sm"> LOG IN </span>
                        </button>
                        <button class="w-30 h-10 bg-[#00B289] rounded-md text-center">
                            <span class="font-bold font-sans text-white text-sm"> START FREE </span>
                        </button>
                    </div>
                </div>
            </section>
            <section class="flex flex-col gap-10 my-10">
                <div class="flex w-full justify-between items-baseline">
                    <div>
                        <h1 class="text-3xl font-serif"> Plans & Pricing </h1>
                    </div>
                    <div class="relative flex gap-4 items-center">
                        <div>
                            <h1 class="text-lg font-sans">
                                MONTHLY
                            </h1>
                        </div>
                        <div class="flex">
                            <label class="inline-flex items-center cursor-pointer">
                                <input type="checkbox" value="" class="sr-only peer">
                                <div class="relative w-9 h-5 bg-[#00B289] peer-focus:outline-none peer-focus:ring-brand-soft dark:peer-focus:ring-brand-soft rounded-full peer peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full peer-checked:after:border-buffer after:content-[''] after:absolute after:top-[2px] after:start-[2px] after:bg-white after:rounded-full after:h-4 after:w-4 after:transition-all peer-checked:bg-brand"></div>
                            </label>
                        </div>
                        <div>
                            <h1 class="text-lg font-sans opacity-50">
                                    YEARLY
                            </h1> 
                        </div>
                        <img class="absolute -top-8 -right-5" src="https://web.archive.org/web/20221117021714im_/https://assets-global.website-files.com/58868bcd2ef4daaf0f072900/5e9d7255d3886a6103fb12a9_FREE-text.svg" alt="2 months free image">
                    </div>
                </div>
                <div class="flex gap-10">
                   <div class="flex-1 flex flex-col p-10 gap-12 border bg-white border-slate-200">
                        <div class="header flex flex-col gap-6">
                            <div>
                                <h2 class="font-semibold font-sans text-2xl">
                                    Workflow
                                </h2>
                            </div>
                            <div class="flex gap-2">
                                <h3 class="text-2xl font-sans">
                                    $
                                </h3>
                                <h1 class="font-bold font-sans text-6xl">
                                    19
                                </h1>
                                <h3 class="self-end-safe text-2xl font-sans">
                                    /MONTH
                                </h3>
                            </div>

                            <hr class="h-0.5 border-t-0 bg-[#00B289]"/>
                        </div> 
                        <div class="body">
                            <ul class="flex flex-col gap-4">
                                <li v-for="list in workflowList" class="flex gap-2">
                                    <Check color="#00B289"/>
                                    <span class="font-sans">
                                        {{  list  }}
                                    </span>
                                </li>
                            </ul>
                        </div>
                        <div class="footer flex justify-center items-center">
                            <button class="w-full h-14 bg-[#00B289] text-center rounded-md">
                                <span class="font-bold font-sans text-white text-lg">
                                    START FREE
                                </span>
                            </button>
                        </div>
                   </div> 
                   <div class="relative overflow-hidden flex-1 flex flex-col p-10 gap-12 border bg-white border-slate-200">
                        <div class="absolute -right-12 top-10 rotate-45 text-center w-60 bg-[#00B289] font-sans font-bold p-2 text-white text-lg uppercase">
                            Most Popular
                        </div>
                        <div class="header flex flex-col gap-6">
                            <div>
                                <h2 class="font-semibold font-sans text-2xl">
                                    Workflow Plus
                                </h2>
                            </div>
                            <div class="flex gap-2">
                                <h3 class="text-2xl font-sans">
                                    $
                                </h3>
                                <h1 class="font-bold font-sans text-6xl">
                                    29
                                </h1>
                                <h3 class="self-end-safe text-2xl font-sans">
                                    /MONTH
                                </h3>
                            </div>

                            <hr class="h-0.5 border-t-0 bg-[#00B289]"/>
                        </div> 
                        <div class="body">
                            <ul class="flex flex-col gap-4">
                                <li v-for="list in workflowPlusList" class="flex gap-2 ">
                                    <Check color="#00B289"/>
                                    <span class="flex gap-2 font-sans" v-if="list.includes('questionnaires')">
                                        {{ list }}
                                        <div class="font-bold font-sans text-white text-sm text-center bg-[#F8DB61] w-10 h-5">
                                            New
                                        </div>
                                    </span>
                                    <span class="font-sans" v-else>
                                        {{   list   }}
                                    </span>
                                </li>
                            </ul>
                        </div>
                        <div class="footer flex justify-center items-center">
                            <button class="w-full h-14 bg-[#00B289] text-center rounded-md">
                                <span class="font-bold font-sans text-white text-lg">
                                    START FREE
                                </span>
                            </button>
                        </div>
                   </div> 
                </div>    
                <div class="flex flex-col gap-10">
                    <div class="flex justify-center items-center">
                        <h1 class="text-2xl font-sans">
                            Super charge your work with add-ons
                        </h1>
                    </div>
                    <div class="flex flex-col gap-4">
                        <div class="flex shadow-sm shadow-gray-300 rounded-md p-10 justify-between">
                            <div class="flex flex-col gap-2">
                                <h1 class="font-semibold font-sans text-xl">
                                    Collaborators
                                </h1>
                                <p class="font-sans">
                                    Invite other users to specific projects for limited access and functionality.
                                </p>
                            </div>
                            <div class="flex flex-col justify-center items-center ">
                                <h1 class="font-semibold font-sans text-3xl">
                                    Free
                                </h1>
                            </div>
                        </div>
                        <div class="flex shadow-sm shadow-gray-300 rounded-md p-10 justify-between">
                            <div class="flex flex-col gap-2">
                                <h1 class="font-semibold font-sans text-xl">
                                    Partners
                                </h1>
                                <p class="font-sans">
                                    Invite other users for full account access and company management
                                </p>
                            </div>
                            <div class="flex flex-col justify-center items-center ">
                                <h1 class="font-semibold font-sans text-3xl">
                                    $9
                                </h1>
                                <h2 class="text-sm font-sans">
                                    /MONTH
                                </h2>
                            </div>
                        </div>
                        <div class="flex shadow-sm shadow-gray-300 rounded-md p-10 justify-between">
                            <div class="flex flex-col gap-2">
                                <h1 class="font-semibold font-sans text-xl">
                                    Bonsai Tax
                                </h1>
                                <p class="font-sans">
                                    Track expenses, indentify write-offs, and estimate quarterly taxes easily.
                                </p>
                                <NuxtLink class="flex font-sans text-[#00B289] items-center" to="/"> 
                                    LEARN MORE 
                                    <ChevronRight :size="18"/>
                                </NuxtLink>
                            </div>
                            <div class="flex flex-col justify-center items-center ">
                                <h1 class="font-semibold font-sans text-3xl">
                                    $10
                                </h1>
                                <h2 class="text-sm font-sans">
                                    /MONTH
                                </h2>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            <section class="flex flex-col justify-center items-center bg-[#F2FAFF] h-80 my-10">
                <div class="flex gap-4 justify-between items-center w-full h-1/2 p-10">
                    <div class="flex flex-2 flex-col font-semibold font-serif text-4xl gap-2">
                        <h1>
                            It's <span class="text-[#00B289]"> your </span> business.
                        </h1>
                        <h1>
                            We're here to help it grow.
                        </h1>
                    </div>
                    <div class="flex-1 flex flex-col justify-center items-center">
                        <button class="w-46 h-14 bg-[#00B289] rounded-md text-center cursor-pointer">
                            <span class="font-bold font-sans text-white text-sm"> START FREE </span>
                        </button>
                    </div>
                </div>
            </section>
            <section class="flex flex-col my-10">
                <div class="text-center">
                    <h1 class="text-2xl font-serif text-[#00B289]">
                        Frequently Asked Questions
                    </h1>
                </div>
                <div class="flex flex-col justify-center gap-4 p-10 px-6">
                    <div v-for="item in faqList" class="flex gap-4 justify-between items-center cursor-pointer">
                        <div>
                            <h1 class="text-2xl font-medium font-sans">
                                {{ item }}
                            </h1>    
                        </div>
                        <ChevronDown />
                    </div>
                </div>
            </section>
        <footer class="flex justify-between my-10">
            <div class="flex flex-col gap-10">
                <h1 class="font-bold font-sans">
                    PRODUCT
                </h1>

                <div class="flex flex-col">
                   <span v-for="item in productList" class="cursor-pointer font-sans">
                        {{ item }}
                   </span>
                   <div class="flex flex-col mt-6">
                        <span class="text-[#00B289] cursor-pointer font-sans">
                            Pricing
                        </span>
                        <span class="cursor-pointer font-sans">
                            Bonsai Reviews
                        </span>
                   </div>
                </div>
            </div>
            <div class="flex flex-col gap-10">
                <h1 class="font-bold font-sans">
                    FREE RESOURCES
                </h1>

                <div class="flex flex-col">
                    <span v-for="item in freeResourcesList" class="cursor-pointer font-sans">
                        {{ item }}
                    </span>
                </div>
                <div class="flex flex-col">
                    <span v-for="item in freeResourcesListTwo" class="cursor-pointer font-sans">
                        {{ item }}
                    </span>
                </div>

                <div class="flex flex-col gap-4">
                    <h1 class="font-bold font-sans">
                        Templates
                    </h1>

                    <div class="flex flex-col">
                        <span v-for="item in templatesList" class="flex items-center cursor-pointer font-sans">
                            {{ item }}
                            <ChevronDown :size="18"/> 
                        </span>
                        <span v-for="item in templatesListTwo" class="flex items-center cursor-pointer font-sans">
                            {{ item }}
                        </span>
                    </div>
                    
                </div>
            </div>
            <div class="flex flex-col gap-10">
                <h1 class="font-bold font-sans">
                    BONSAI
                </h1>

                <div class="flex flex-col">
                    <span v-for="item in bonsaiList" class="flex cursor-pointer font-sans">
                        {{ item }}
                    </span>
                </div>
                <div class="flex flex-col">
                    <span v-for="item in bonsaiListTwo" class="cursor-pointer font-sans">
                        {{ item }}
                    </span>
                </div>
                <span class="flex items-center cursor-pointer font-sans">
                    Comparisons
                    <ChevronDown :size="18"/>
                </span>
            </div>
        </footer>
        </div>
    </div>
</template>

<script lang="ts" setup>
import { ChevronDown, ChevronRight, Flower, Check } from '@lucide/vue';

const workflowList = [
    "Unlimited Clients & Projects",
    "Proposals",
    "Contracts",
    "Invoicing & Payments",
    "Client CRM",
    "Project Management",
    "Task & Time Tracking",
    "iOS, Android, Chrome, Mac Apps"
];

const workflowPlusList: string[] = [
    "Everything in Workflow, plus...",
    "White-labelled client experience",
    "Client forms and questionnaires",
    "Workflow automations",
    "Subcontracting (client-mode)",
    "Calendly Integration",
    "Client portal",
    "Priority support"
];

const faqList: string[] = [
    "How does the 14 day free trial work?",
    "Can I change plans anytime?",
    "How do I pause my Bonsai subscription?",
    "What is your refund policy?",
];

const productList: string[] = [
    "Proposals",
    "Contracts",
    "Invoicing",
    "Client CRM",
    "Time Tracking",
    "Task Tracking",
    "Forms",
    "Accounting",
    "Bonsai Tax",
    "Bonsai Cash",
];

const freeResourcesList: string[] = [
    "Freelance Resources",
    "Freelance Blogn by Bonsai",
    "How to Write a Contract",
    "Online Signature Maker"
];

const freeResourcesListTwo: string[] = [
    "Self-Employed Taxes Hub",
    "Self-Employed Tax Calculator",
    "Self-Employed Tax Deductions",
];

const templatesList: string[] = [
    "Invoice Templates",
    "Proposal Templates",
    "Contract Templates",
    "Agreement Templates",
    "Scope of Work Templates",
    "Quote Templates",
];

const templatesListTwo: string[] = [
    "Credit Note Templates",
    "Estimate Templates",
    "Form Templates",
];

const bonsaiList: string[] = [ 
    "About",
    "Careers",
    "Support",
    "LinkedIn",
    "Twitter",
    "Privacy Policy",
    "Legal",
];

const bonsaiListTwo: string[] = [
    "Affiliates",
    "Write for Us"
];

</script>