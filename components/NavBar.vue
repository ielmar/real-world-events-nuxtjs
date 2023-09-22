<template>
  <div class="ml-10 flex items-baseline space-x-4">
    <a
      v-for="item in navigation"
      :key="item.name"
      :href="item.href"
      :class="[
        item.current
          ? 'bg-gray-900 text-white'
          : 'text-gray-300 hover:bg-gray-700 hover:text-white',
        'rounded-md px-3 py-2 text-sm font-medium',
      ]"
      :aria-current="item.current ? 'page' : undefined"
      >{{ item.name }}</a
    >
  </div>
</template>

<script setup>
const navigation = [
  { name: 'Events', href: '/', current: true },
  { name: 'Create Event', href: '/create', current: false },
]
</script>
