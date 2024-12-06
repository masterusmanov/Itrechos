<template>
  <div class="my-[40px]">
    <div class="container mx-auto">
      <div id="accordion-color" data-accordion="collapse" data-active-classes="">
          <div v-for="(item, index) in accordionItems" :key="index" class="border-b border-[#FF8911]">
            <h2 :id="`accordion-color-heading-${index + 1}`">
              <button
                type="button"
                class="flex items-center justify-between w-full p-5 text-[16px] md:text-[24px] font-[700] text-left"
                :data-accordion-target="`#accordion-color-body-${index + 1}`"
                :aria-expanded="activeAccordionId === index + 1"
                :aria-controls="`accordion-color-body-${index + 1}`"
                @click="toggleAccordion(index + 1)"
              >
                <span>{{ item.title }}</span>
                <svg
                  data-accordion-icon
                  class="w-3 h-3 rotate-180 shrink-0"
                  aria-hidden="true"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 10 6"
                >
                  <path
                    stroke="currentColor"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 5 5 1 1 5"
                  />
                </svg>
              </button>
            </h2>
            <div
              :id="`accordion-color-body-${index + 1}`"
              :class="{ 'hidden': activeAccordionId !== index + 1 }"
              :aria-labelledby="`accordion-color-heading-${index + 1}`"
            >
              <div class="px-[20px]">
                <p class="">
                  {{ item.content }}
                </p>
              </div>
            </div>
          </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const activeAccordionId = ref(null);

const toggleAccordion = (id) => {
  activeAccordionId.value = activeAccordionId.value === id ? null : id;
};

const accordionItems = [
  {
    title: 'An Award winning company',
    content: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before. Holistic deliver end sound benefits. ',
  },
  {
    title: 'Quick Research and Solutions',
    content: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before. Holistic deliver end sound benefits. ',
  },
  {
    title: 'Dedicated Support 24/7',
    content: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before. Holistic deliver end sound benefits. ',
  },
  {
    title: 'Quick Support & Tech Solution',
    content: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before. Holistic deliver end sound benefits. ',
  }
];
</script>