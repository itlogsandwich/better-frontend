<template>
    <div class="min-h-screen flex justify-center">
        <div class="min-h-full w-full flex flex-col border">
            <nav class="flex justify-between py-4 px-14 bg-black items-center">
                <section class="flex gap-4 text-white">
                    <div class="flex gap-2 items-center">
                        <Icon name="heroicons-solid:inbox-stack"
                        size="30" 
                        />
                        <h1> Abstract </h1>
                    </div>
                    <span> | </span>
                    <h1>
                        Help Center
                    </h1>
                </section>

                <section class="flex gap-4">
                    <button type="button" class="w-40 h-10 border border-white bg-black text-white text-center rounded-md">
                        Submit a Request
                    </button>
                    <button type="button" class="w-20 h-10 bg-[#4c5fd5] text-white text-center rounded-md ">
                        Sign In
                    </button>
                </section>
            </nav>

            <header class="flex w-full h-80 justify-center items-center bg-[#dadbf1]">
                <section class="flex flex-col gap-10">
                    <label class="font-medium text-7xl" for="search">
                        How can we help?
                    </label>
                    <input class="w-full h-10 shadow-sm shadow-gray-200 px-4 focus:outline-none bg-white" type="text" id="search" name="search" placeholder="Search"/>
                </section>
            </header>

            <main class="flex gap-4 w-full justify-center items-center mt-10 p-10">
               <section class="flex flex-col gap-10">
                    <Item class="flex-1" v-for="item in colOne" :icon="item.icon" :title="item.title" :description="item.description" />
               </section> 
               <section class="flex flex-col gap-10">
                    <Item class="flex-1" v-for="item in colTwo" :icon="item.icon" :title="item.title" :description="item.description" />
               </section>
            </main>
            <footer class="flex gap-10 h-80 py-4 px-14 bg-black text-white justify-evenly">
                <section class="flex flex-col gap-2">
                    <h3 class="font-bold text-xl">
                        Abstract
                    </h3>
                    <span> Branches </span>
                </section>

                <section class="flex flex-col gap-2">
                    <h3 class="font-bold text-xl">
                        Resources
                    </h3>
                    <ul v-for="item in listOne" >
                        <li>
                            {{ item }}
                        </li>
                    </ul>
                </section>

                <section class="flex flex-col gap-2">
                    <h3 class="font-bold text-xl">
                        Community
                    </h3>
                    <ul v-for="item in listTwo" >
                        <li>
                            {{ item }}
                        </li>
                    </ul>
                </section>

                <section class="flex flex-col gap-6">
                    <div class="flex flex-col gap-2">
                        <h3 class="font-bold text-xl">
                            Company
                        </h3>
                        <ul v-for="item in listThree" >
                            <li>
                                {{ item }}
                            </li>
                        </ul>
                    </div>
                    <div class="flex flex-col gap-2">
                        <h5 class="font-bold">
                            Contact Us
                        </h5>
                        <span> info@abstract.com </span>
                    </div>
                </section>

                <section class="flex flex-col justify-end">
                    <Icon name="heroicons-solid:inbox-stack"
                    size="30" />
                    <div class="flex flex-col">
                        <h2>
                            Copyright 2022
                        </h2>
                        <h2>
                            Abstract Studio Design, Inc.
                        </h2>
                        <h2>
                            All rights reserved
                        </h2>
                    </div>
                </section>
            </footer>
        </div>
    </div>
</template>
<script lang="ts" setup>

const colOne = [
   {
        icon: "heroicons-solid:link",
        title: "Branches",
        description: "Abstract Branches lets you manage, version, and document your designs in one place." 
   },
   {
        icon:"heroicons-solid:puzzle",
        title: "Manage organizations, teams, and projects",
        description: "Use Abstract organizations, teams, and projcets to organize your people and your work."
   },
   {
        icon:"heroicons-solid:key",
        title: "Authenticate to Abstract",
        description: "Set up and configure SSO, SCIM, and Just-in-Time provisioning.",
   }
];

const colTwo = [
   {
        icon:"heroicons-solid:users",
        title: "Manage your account",
        description: "Configure your account settings, such as your email, profile details, and password." 
   },
   {
        icon:"heroicons-solid:currency-dollar",
        title: "Manage billing",
        description: "Change subscriptions and payment details."
   },
   {
        icon:"heroicons-solid:chat-alt",
        title: "Abstract support",
        description: "Get in touch with a human",
   }
]

const listOne = [
   "Blog",
   "Help Center",
   "Release Notes",
   "Status",
];

const listTwo = [
   "Twitter",
   "LinkedIn",
   "Facebook",
   "Dribbble",
   "Podcast",
];

const listThree = [
    "About Us",
    "Careers",
    "Legal"
];
</script>