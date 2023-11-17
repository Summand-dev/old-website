<template>
  <Header />
  <section class="h-screen">
    <h2 class="text-center text-3xl md:text-6xl font-semibold dark:text-white">How To Install</h2>
    <div class="flex items-center justify-center">
    <div class="w-full max-w-md px-2 py-16 sm:px-0">
      <TabGroup>
        <TabList class="flex space-x-1 rounded-xl p-1">
          <Tab v-for="category in Object.keys(categories)" as="template" :key="category" v-slot="{ selected }">
            <button :class="[
              'w-full py-2.5 text-sm font-medium leading-5',
              // 'ring-white/60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2',
              selected
                ? 'text-blue-700  border-b-2 dark:border-white dark:text-white'
                : 'text-[#5C6280] dark:text-white',
            ]">
              {{ category }}
            </button>
          </Tab>
        </TabList>

        <TabPanels class="mt-2">
          <TabPanel v-for="(posts, idx) in Object.values(categories)" :key="idx" :class="[
            'rounded-xl bg-white p-3 border-2 dark:bg-[#08102B] dark:border-[#192245] dark:text-white',
            'ring-white/60 ring-offset-2 ring-offset-blue-400 focus:outline-none focus:ring-2',
          ]">
            <ul>
              <li v-for="post in posts" :key="post.id" class="relative rounded-md p-3">
                <h3 class="text-sm font-medium leading-5">
                  {{ post.description }}
                </h3>
              </li>
            </ul>
          </TabPanel>
        </TabPanels>
      </TabGroup>
    </div>
  </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from '@headlessui/vue'
import Header from '@/components/Header.vue'

const categories = ref({
  Windows: [
    {
      description: 'pip install summand',
    }
  ],
  Linux: [
    {
      description: 'pip install summand',
    }
  ],
  MacOS: [
    {
      description: 'pip install summand',
    }
  ],
})
</script>
