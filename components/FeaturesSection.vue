<template>
    <div class="w-full flex justify-center">
        <div class="absolute w-full h-96" style="background: linear-gradient(180deg, rgba(24,24,27,1) 0%, rgba(9,9,11,1) 100%);"></div>
        <ULandingSection 
            class="px-8 py-32 max-w-7xl h-content z-10"
            title="Whats Included?"
            description="This project is an experiment to see how a modern app, with features like auth, subscriptions, API routes, and static pages would work in Next.js 13 app dir."
       >
            <ULandingGrid>
                <ULandingCard class="col-span-4 row-span-2" icon="i-heroicons-swatch" title="Nuxt 3.14" description="Choose a primary and a gray color from your Tailwind CSS color palette." />
                <ULandingCard class="col-span-4 row-span-2" icon="i-heroicons-wrench-screwdriver" title="Fully Customizable" description="Change the style of any component in your App Config or with ui prop." />
                <ULandingCard class="col-span-4 row-span-2" icon="i-heroicons-face-smile" title="Icons" description="Choose any of the 100k+ icons from the most popular icon libraries." />
                <ULandingCard class="col-span-4 row-span-2" icon="i-heroicons-computer-desktop" title="Keyboard Shortcuts" description="Nuxt UI comes with a set of Vue composables to easily handle shortcuts." />
                <ULandingCard class="col-span-4 row-span-2" icon="i-heroicons-face-smile" title="Icons" description="Choose any of the 100k+ icons from the most popular icon libraries." />
                <ULandingCard class="col-span-4 row-span-2" icon="i-heroicons-computer-desktop" title="Keyboard Shortcuts" description="Nuxt UI comes with a set of Vue composables to easily handle shortcuts." />
            </ULandingGrid>
        </ULandingSection>
    </div>
  </template>