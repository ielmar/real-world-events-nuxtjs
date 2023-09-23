<template>
  <div>
    <header class="bg-[#E87121]">
      <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="flex h-16 items-center justify-between">
          <div class="flex items-center">
            <div class="flex-shrink-0">
              <nuxt-link to="/">
                <img
                  class="h-12 w-12"
                  src="~/static/logo.svg"
                  alt="Your Company"
                />
              </nuxt-link>
            </div>
            <div class="hidden md:block">
              <NavBar />
            </div>
          </div>
        </div>
      </div>
    </header>
    <header class="bg-white shadow">
      <div class="mx-auto max-w-7xl px-4 py-6 sm:px-6 lg:px-8">
        <h1 class="text-3xl font-bold tracking-tight text-gray-900">Events</h1>
      </div>
    </header>
    <main>
      <div class="mx-auto max-w-7xl py-6 sm:px-6 lg:px-8"><slot /></div>
    </main>
  </div>
</template>
<script>
import NavBar from '~/components/NavBar.vue'
export default {
  components: {
    NavBar,
  },
}
</script>
