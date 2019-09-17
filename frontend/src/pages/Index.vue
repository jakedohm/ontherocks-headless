<template>
  <div class="bg-grey-lighter">
    <div id="body-container">
      <div id="nav" class="border-b border-grey-light">
        <div
          class="container mx-auto flex items-center justify-between flex-wrap px-6 py-4"
        >
          <a class="flex items-center flex-no-shrink no-underline" href="/">
            <img
              class="h-8 w-8 mr-2"
              src="/images/logo.svg"
              alt="On the Rocks Logo"
            />
            <h1 class="font-semibold text-xl text-grey-darkest tracking-tight">
              On the Rocks
            </h1>
          </a>
          <div class="hidden md:block md:flex-grow"></div>
        </div>
      </div>

      <main>
        <div class="bg-grey-light py-6 br rounded">
          <div class="container mx-auto px-6">
            <div class="md:flex -mx-4">
              <div class="flex mb-1 md:mb-0 mx-4 w-full">
                <input
                  id="search"
                  class="text-input rounded-r-none"
                  type="text"
                  placeholder="Search by keyword"
                />
                <button class="-ml-1 px-4 rounded-r bg-blue-dark text-white">
                  Search
                </button>
              </div>
            </div>
          </div>
        </div>

        <div class="container py-8 mx-auto px-6">
          <div id="recipe-list" class="flex flex-wrap -mx-4">
            <Recipe v-for="index in 10" :key="index" />
          </div>
        </div>
      </main>
    </div>
  </div>
</template>

<script>
import Recipe from '@/components/Recipe'

export default {
  components: {
    Recipe,
  },
}
</script>
