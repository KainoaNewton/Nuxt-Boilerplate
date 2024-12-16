<template>
    <AuroraBackground>
        <div
        v-motion
        :initial="{ opacity: 0, y: 40 }"
        :visible="{
            opacity: 1,
            y: 0,
            transition: {
            delay: 0.3,
            duration: 0.8,
            ease: 'easeInOut',
            },
        }"
        class="relative flex flex-col items-center justify-center gap-4 px-8 max-w-7xl"
        >
        <ULandingSection
        title="The freedom to build anything"
        description="Nuxt UI Pro ships with an extensive set of advanced components that cover a wide range of use-cases."
        :links="[{ label: 'Features', trailingIcon: 'i-heroicons-arrow-right', size: 'xl', to: '#features' },{ label: 'Use this template', color: 'gray', icon: 'i-simple-icons-github', size: 'xl', target: '_blank', to: 'https://github.com/nuxt-ui-pro/landing' }]"
        />
        </div>
    </AuroraBackground>
  </template>