<template>
  <nav class="ml-5 mt-5 relative border-l border-gray-700">
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
</nav>
</template>

<style scoped>
body {
  margin: auto;
  padding: auto;
}

.nuxt-link-active {
  color: gray;
}
</style>
