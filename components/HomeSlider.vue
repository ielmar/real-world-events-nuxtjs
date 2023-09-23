<template>
  <div class="flex mb-10">
    <div v-for="item in items" :key="item.id" class="">
      <img :src="item.image" alt="item.title" class="w-full" />
    </div>
  </div>
</template>

<script setup>
const items = [
  {
    id: 1,
    name: 'Party',
    href: '/',
    current: true,
    image:
      'https://images.unsplash.com/photo-1501281668745-f7f57925c3b4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=4140&q=80',
  },
]
</script>
