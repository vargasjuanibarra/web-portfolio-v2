<template>
    <div class="grid py-8 md:px-2 md:py-12 text-white">
        <div class="text-white text-center mb-8 md:pb-12">
            <p class="text-2xl font-semibold">a few of my creative endeavors.</p>
            <h2 class="text-2xl font-semibold text-wrap md:text-4xl lg:text-5xl">Curious to <span class="text-emerald-400">see</span> my work?</h2>
        </div>
        <div class="grid gap-5  p-4 sm:grid-cols-2 lg:grid-cols-3">
            <div class="relative border rounded-lg my-4 hover:border-gray-600 duration-200 items-center" v-for="project, index in projects" :key="index">
                <font-awesome-icon :icon="project.icon" size="2xl" class="p-4 bg-slate-900 absolute -top-8"/>
                <div class="p-4">
                    <p class="text-center text-xl font-semibold py-2">{{project.title}}</p>
                    <p class="text-center md:text-md lg:text-lg"> {{project.description}} </p>
                    <p class="text-center md:text-md lg:text-lg text-emerald-400 font-semibold"> {{project.stack}} </p>
                </div>
                <div class="flex justify-between pt-12 items-center">
                    <a :href="project.repo" class="absolute bottom-0 left-0 right-2 p-4 rounded-lg" >
                        <font-awesome-icon :icon="['fab', 'github']" size="2xl" class="hover:scale-110 transform-transition duration-200 easi-in-out"/>
                    </a>
                    <a :href="project.link" class="absolute bottom-0 right-0 rounded-lg" >
                        <div class="ml-auto cursor-pointer rounded-md p-2 hover:text-slate-950 duration-200 hover:bg-emerald-400  relative after:absolute after:top-0 after:h-0 after:right-full after:w-full after:h-full after:bg-white after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden">
                            <p class="relative p-2 z-4">Go to &rarr;</p>
                        </div>
                    </a>
                </div>
                
            </div>

        </div>
    </div>

</template>
<script setup>
    const projects = [
        { 
            id: 1,
            title: 'E-commerce Store',
            icon: 'cart-shopping',
            description: 'The e-commerce website I developed serves as a testament to my ability to construct an application from scratch, while simultaneously mastering the SvelteKit framework. This project underscores my commitment to continuous learning and professional growth in web development.',
            stack: 'Typescript, SvelteKit, Tailwind',
            link: 'https://supremesalestation.netlify.app/',
            repo: 'https://github.com/vargasjuanibarra/ecommerce-website'
        },
        { 
            id: 2,
            title: 'Expense Tracker',
            icon: 'calculator',
            description: 'The expense tracker website I developed showcases my expertise in Vue.js by refreshing my knowledge through creating an application from scratch. This project underscores my commitment to continuous learning and my ability to design efficient web applications.',
            stack: 'Vue, Typescript, CSS',
            link: 'https://juanexpensetracker.netlify.app/',
            repo: 'https://github.com/vargasjuanibarra/expense-tracker-vue'
        },
        { 
            id: 3,
            title: 'Online Image Finder',
            icon: 'image',
            description: 'The online image finder website I developed, harnessing the basics of Svelte, Tailwind CSS, and an image finder API, demonstrates my capability to integrate various technologies effectively. This project underscores my commitment to professional growth and technical adaptability.',
            stack: 'Svelte, Tailwind, Javascript',
            link: 'https://onlineimagefinder.netlify.app/',
            repo: 'https://github.com/vargasjuanibarra/online-image-gallery-finder'
        },
        { 
            id: 4,
            title: 'PokeDex Website',
            icon: 'tablet-screen-button',
            description: 'The Pokedex website I developed exemplifies my proficiency in using API data and creating applications from scratch, while concurrently learning the SvelteKit and tailwind frameworks. This project highlights my dedication to professional development and mastery in web application design.',
            stack: 'Javascript, SvelteKit, Tailwind',
            link: 'https://juanpokemonmaster.netlify.app/',
            repo: 'https://github.com/vargasjuanibarra/pokedex-webapp'
        },
        { 
            id: 5,
            title: 'E-commerce Store',
            icon: 'fa-regular fa-cart-shopping',
            description: 'The e-commerce website I developed serves as a testament to my ability to construct an application from scratch, while simultaneously mastering the SvelteKit framework. This project underscores my commitment to continuous learning and professional growth in web development.'
        },
        { 
            id: 6,
            title: 'E-commerce Store',
            icon: 'fa-regular fa-cart-shopping',
            description: 'The e-commerce website I developed serves as a testament to my ability to construct an application from scratch, while simultaneously mastering the SvelteKit framework. This project underscores my commitment to continuous learning and professional growth in web development.'
        },
    ]
</script>
<style lang="">
    
</style>