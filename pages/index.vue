<template>
<ol class="relative ml-5 mt-5 text-gray-500" 
>                  
    <li class="p-10 cursor-pointer border-l-2" @click="changeStep(1)" :class="[ step === 1 ? 'border-blue-400 text-black' :  'border-gray-200 text-gray-400' ]">
      <span class="flex flex-row gap-5">
        <!-- <span class="absolute flex items-center justify-center w-8 h-8 bg-green-200 rounded-full -left-4 ring-4 ring-white dark:ring-gray-900 dark:bg-green-900"> -->
            <svg v-if="step === 1"  class=" bg-blue-500 text-white w-8 h-8 rounded-full" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
            <svg v-else class="bg-gray-500 text-blue-500 w-8 h-8 rounded-full" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
        <!-- </span> -->

        <span>
        <h3 class="text-lg font-semibold">
          Save Content
        </h3>
        <p class="mb-4 text-base font-normal">
          Use Inga to save links or upload your files in any format (jpg, mp4, pdf & more)
        </p>
      </span>
        </span>            
    </li>
    <li class="p-10 cursor-pointer border-l-2" @click="changeStep(2)" :class="[ step === 2 ? 'border-blue-400 text-black' :  'border-gray-200 text-gray-400' ]">
      <span class="flex flex-row gap-5" >
        <!-- <span class="absolute flex items-center justify-center w-8 h-8 bg-green-200 rounded-full -left-4 ring-4 ring-white dark:ring-gray-900 dark:bg-green-900"> -->
          <svg v-if="step ===2"  class=" bg-blue-500 text-white w-8 h-8 rounded-full" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
            <svg v-else class="bg-gray-500 text-blue-500 w-8 h-8 rounded-full" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
        <!-- </span> -->

        <span>
          <h3 class="text-lg font-semibold">
      Save Browser Tabs
    </h3>
    <p class="mb-4 text-base font-normal">
      Save an entire web session with the tab collector & reopen it easily later.
    </p>
      </span>
        </span>            
    </li>
    <li class="p-10 cursor-pointer border-l-2" @click="changeStep(3)" :class="[ step === 3 ? 'border-blue-400 text-black' :  'border-gray-200 text-gray-400' ]">
      <span class="flex flex-row gap-5">
        <!-- <span class="absolute flex items-center justify-center w-8 h-8 bg-green-200 rounded-full -left-4 ring-4 ring-white dark:ring-gray-900 dark:bg-green-900"> -->
          <svg v-if="step ===3"  class=" bg-blue-500 text-white w-8 h-8 rounded-full" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
            <svg v-else class="bg-gray-500 text-blue-500 w-8 h-8 rounded-full" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
        <!-- </span> -->

        <span>
          <h3 class="text-lg font-semibold">
      Organize
    </h3>
    <p class="mb-4 text-base font-normal">
      Use collections to curate your content into different themes or projects. Group content into folders within a collection.
    </p>
      </span>
        </span>            
    </li>
   
</ol>

</template>

<script setup>
import {ref} from "vue"

const step = ref(1)


function changeStep(stepVal){
  step.value = stepVal
  console.log(step.value)
  console.log("Hey it clicked")
}
// const changeStep(stepVal) => {step.value = stepVal}

</script>

<style scoped>
body {
  margin: auto;
  padding: auto;
}

.nuxt-link-active {
  color: gray;
}
</style>
