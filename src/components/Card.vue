<template>
  <div class="flex rounded shadow-lg overflow-hidden">
    <img :src="cardData.image" alt=""
      class="w-32 h-32 object-cover object-center"
    >
    <div class="ml-4 py-4 flex flex-col">
      <h2 class="font-bold text-xl">{{ cardData.city }}</h2>
      <p class="text-gray-600">${{ cardData.price }} / night average</p>
      <a href="#" class="text-indigo-600 mt-auto">Explore {{cardData.propCount}} properties</a>
    </div>
  </div>
</template>

<script>
  export default {
    props: ['cardData']
  }
</script>
