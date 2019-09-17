<template>
  <div class="bg-grey-lighter cover-image">
    <div
      id="cover-image"
      style="background-image: url('/images/recipe-bg-placeholder.jpg')"
    ></div>

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
        <div class="container mx-auto px-6">
          <div class="flex flex-wrap lg:-mx-6 py-12">
            <div class="w-full lg:w-3/5 lg:px-6">
              <div
                id="recipe"
                class="text-grey-darkest rounded shadow-lg bg-white mb-12"
              >
                <div class="shadow p-8 md:p-16">
                  <img
                    class="block w-32 h-32 object-cover rounded mx-auto mb-8 lg:float-right lg:ml-16 lg:mb-16"
                    src="https://via.placeholder.com/400"
                  />

                  <h1
                    class="page-heading mt-4 pb-2 border-b-4 border-grey-lighter text-center lg:text-left"
                  >
                    Gin Martini
                  </h1>

                  <ul class="list-reset mb-6">
                    <li class="mb-1 font-bold">Ingredient #1</li>
                    <li class="mb-1 font-bold">Ingredient #2</li>
                    <li class="mb-1 font-bold">Ingredient #3</li>
                  </ul>

                  <ol class="list-reset">
                    <li class="mb-2">Step #1</li>
                    <li class="mb-2">Step #2</li>
                    <li class="mb-2">Step #3</li>
                  </ol>
                </div>
              </div>

              <div
                class="rounded bg-grey-light p-8 md:p-16 leading-normal text-grey-darkest description"
              >
                This is a test description. Replace me with the real
                description.
              </div>
            </div>
            <div class="w-full lg:w-2/5 lg:px-6 text-grey-darker text-sm">
              <div class="rounded border border-grey mb-8">
                <div class="glass-type px-4 py-6 flex items-center">
                  <div class="w-1/2 pr-8 text-right">Serve in</div>
                  <div class="-ml-6 mr-1">
                    <GlassIcon glass="martini" />
                  </div>
                  <span>Martini Glass</span>
                </div>
                <div class="border-t border-grey px-4 py-6 flex items-center">
                  <div class="w-1/2 pr-8 text-right">Submitted by</div>
                  <div class="-ml-6 mr-1">
                    <img
                      src="/images/user.svg"
                      alt="Jane Doe"
                      class="block w-12 h-12 rounded-full shadow mr-2"
                    />
                  </div>
                  <span>Jane Doe</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </main>
    </div>
  </div>
</template>

<script>
import GlassIcon from '@/components/GlassIcon'

export default {
  components: {
    GlassIcon,
  },
}
</script>
