<script setup lang="ts">
const { data: page } = await useAsyncData('index', () => queryContent('/').findOne())

useSeoMeta({
  title: page.value.title,
  ogTitle: page.value.title,
  description: page.value.description,
  ogDescription: page.value.description
})
</script>

<template>
    <UMain>
      <div class="relative flex flex-col items-center justify-center h-screen">
        <FallingStarsBg class="bg-black" />
        <div class="z-[1] flex items-center">
          <div class="flex justify-center items-center"></div>
            <ULandingSection
              title="The freedom to build anything"
              description="Nuxt UI Pro ships with an extensive set of advanced components that cover a wide range of use-cases."
              :links="[{ label: 'Explore components', color: 'gray', trailingIcon: 'i-heroicons-arrow-right', size: 'lg' }]"
            >
            <template #headline>
              <UBadge
                v-if="page.hero.headline"
                variant="subtle"
                size="lg"
                class="relative rounded-full font-semibold"
              >
                <NuxtLink
                  :to="https://ui.nuxt.com/pro"
                  target="_blank"
                  class="focus:outline-none"
                  tabindex="-1"
                >
                  <span
                    class="absolute inset-0"
                    aria-hidden="true"
                  />
                </NuxtLink>

                Made with Nuxt UI Pro

                <UIcon
                  v-if="i-heroicons-arrow-top-right-on-square-20-solid"
                  :name="i-heroicons-arrow-top-right-on-square-20-solid"
                  class="ml-1 w-4 h-4 pointer-events-none"
                />
              </UBadge>
            </template>
          </ULandingSection>
        </div>
      </div>
    </UMain>
</template>