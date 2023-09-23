<template>
  <div class="bg-white mt-20">
    <h2 class="text-2xl font-bold tracking-tight text-gray-900">
      Incoming Events
    </h2>

    <div
      class="mt-6 grid grid-cols-1 gap-x-6 gap-y-10 sm:grid-cols-2 lg:grid-cols-4 xl:gap-x-8"
    >
      <div v-for="event in events" :key="event.id" class="group relative">
        <div
          class="aspect-h-1 aspect-w-1 w-full overflow-hidden rounded-md bg-gray-200 lg:aspect-none group-hover:opacity-75 lg:h-80"
        >
          <img
            :src="event.imageSrc"
            :alt="event.imageAlt"
            class="h-full w-full object-cover object-center lg:h-full lg:w-full"
          />
        </div>
        <div class="mt-4 flex justify-between">
          <div>
            <h3 class="text-sm text-gray-700">
              <a :href="event.href">
                <span aria-hidden="true" class="absolute inset-0" />
                {{ event.name }}
              </a>
            </h3>
            <p class="mt-1 text-sm text-gray-500">{{ event.venue }}</p>
          </div>
          <p class="text-sm font-medium text-gray-900">{{ event.price }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const events = [
  {
    id: 1,
    name: 'Dance till the morning',
    href: '#',
    imageSrc:
      'https://images.unsplash.com/photo-1549451371-64aa98a6f660?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=4140&q=80',
    imageAlt: "Front of men's Basic Tee in black.",
    price: '$35',
    venue: 'Savaya Club',
  },
  {
    id: 2,
    name: 'Basic Tee',
    href: '#',
    imageSrc:
      'https://images.unsplash.com/photo-1643759543584-fb6f448d42d4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=4144&q=80',
    imageAlt: "Front of men's Basic Tee in black.",
    price: '$35',
    venue: 'Black',
  },
  {
    id: 3,
    name: 'Basic Tee',
    href: '#',
    imageSrc:
      'https://images.unsplash.com/photo-1601601392622-5d18104a78fe?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=4140&q=80',
    imageAlt: "Front of men's Basic Tee in black.",
    price: '$35',
    venue: 'Black',
  },
  {
    id: 4,
    name: 'Basic Tee',
    href: '#',
    imageSrc:
      'https://plus.unsplash.com/premium_photo-1661306543132-93937b4c242e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=3000&q=80',
    imageAlt: "Front of men's Basic Tee in black.",
    price: '$35',
    venue: 'Black',
  },
]
</script>
