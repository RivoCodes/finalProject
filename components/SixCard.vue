<template>
  <h1 class="text-2xl font-bold mb-2">{{ data.name }}</h1>
  <p class="text-1xl text-gray-500 mb-4">{{ data.detail }}</p>
  <div class="pb-4 flex items-center flex-col ">
    <img :src="data.img" class="w-full h-80 object-cover block" alt="AIRBNB"/>
    <NuxtLink to="/" class=" mt-4 hover:scale-x-110 transition-all ease">
      <div class="">
        <span>Découvrir des logements</span>
        
      </div>
    </NuxtLink>
  </div>
</template>

<script>
export default {
    name: 'SixCard',
    props: {
        data: Object
    }
}
</script>