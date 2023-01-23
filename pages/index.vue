<template>
  <!-- <nav class="ml-5 mt-5 relative border-l border-gray-700">
  <div class=" ">
    
    <NuxtLink to="" class="flex flex-row gap-5 mb-10 ml-4 cursor-pointer" exact>
      <i class="text-blue-500">icon</i>
      <span>
        <h3 class="text-lg font-semibold text-black">
          Save Content
        </h3>
        <p class="mb-4 text-base font-normal text-gray-500">
          Use Inga to save links or upload your files in any format (jpg, mp4, pdf & more)
        </p>
      </span>
    </NuxtLink>
   
    <NuxtLink to="" class="flex flex-row gap-5 mb-10 ml-4 cursor-pointer">
  <i>icon</i>
  <div>
    <h3 class="text-lg font-semibold text-gray-500">
      Save Browser Tabs
    </h3>
    <p class="mb-4 text-base font-normal text-gray-500 ">
      Save an entire web session with the tab collector & reopen it easily later.
    </p>
  </div>
</NuxtLink>



<NuxtLink to="" class="flex flex-row gap-5 mb-10 ml-4 cursor-pointer">
  <i>icon</i>
  <div>
    <h3 class="text-lg font-semibold text-gray-500">
      Organize
    </h3>
    <p class="mb-4 text-base font-normal text-gray-500 ">
      Use collections to curate your content into different themes or projects. Group content into folders within a collection.
    </p>
  </div>
</NuxtLink>
  </div>
</nav> -->


<ol class="relative ml-5 mt-5 text-gray-500 border-l-2 border-gray-200 " 
>                  
    <li class="mb-10 ml-6" @click="changeStep(1)" :class="[ ifActive ? 'border-blue-200 text-black' :  'border-gray-200 text-gray-200' ]">
      <span class="flex flex-row gap-5 cursor-pointer" >
        <!-- <span class="absolute flex items-center justify-center w-8 h-8 bg-green-200 rounded-full -left-4 ring-4 ring-white dark:ring-gray-900 dark:bg-green-900"> -->
            <svg aria-hidden="true"  class=" bg-blue-500 text-white w-8 h-8 rounded-full" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
        <!-- </span> -->

        <span>
        <h3 class="text-lg font-semibold text-black">
          Save Content
        </h3>
        <p class="mb-4 text-base font-normal text-black">
          Use Inga to save links or upload your files in any format (jpg, mp4, pdf & more)
        </p>
      </span>
        </span>            
    </li>
    <li class="mb-10 ml-6 cursor-pointer" @click="changeStep(2)" :class="[ ifActive ? 'border-blue-200 text-black' :  'border-gray-200 text-gray-200' ]">
      <span class="flex flex-row gap-5" >
        <!-- <span class="absolute flex items-center justify-center w-8 h-8 bg-green-200 rounded-full -left-4 ring-4 ring-white dark:ring-gray-900 dark:bg-green-900"> -->
            <svg aria-hidden="true" class=" bg-blue-200 text-blue-500 w-8 h-8 rounded-full" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
        <!-- </span> -->

        <span>
          <h3 class="text-lg font-semibold text-gray-500">
      Save Browser Tabs
    </h3>
    <p class="mb-4 text-base font-normal text-gray-500 ">
      Save an entire web session with the tab collector & reopen it easily later.
    </p>
      </span>
        </span>            
    </li>
    <li class="mb-10 ml-6 cursor-pointer" @click="changeStep(3)" :class="[ ifActive ? 'border-blue-200 text-black' :  'border-gray-200 text-gray-200' ]">
      <span class="flex flex-row gap-5">
        <!-- <span class="absolute flex items-center justify-center w-8 h-8 bg-green-200 rounded-full -left-4 ring-4 ring-white dark:ring-gray-900 dark:bg-green-900"> -->
            <svg aria-hidden="true" class=" bg-blue-200 text-blue-500 w-8 h-8 rounded-full" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M16.707 5.293a1 1 0 010 1.414l-8 8a1 1 0 01-1.414 0l-4-4a1 1 0 011.414-1.414L8 12.586l7.293-7.293a1 1 0 011.414 0z" clip-rule="evenodd"></path></svg>
        <!-- </span> -->

        <span>
          <h3 class="text-lg font-semibold text-gray-500">
      Organize
    </h3>
    <p class="mb-4 text-base font-normal text-gray-500 ">
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
const ifActive = ref(false)

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
