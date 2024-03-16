<script setup>
const input = defineModel()

</script>

<template>
  <div class="flex flex-row gap-2">
    <input id="APIInput" class=" border-2 p-4 bg-zinc-100 rounded-full  h-14 focus:shadow-2xl"
      placeholder="Enter API" v-model="input" />

    <button @click="$emit('showSearch')"
      class="border-2 rounded-full h-14 w-14 p-2 flex items-center justify-center bg-black">
      <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="white"
        stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-check">
        <polyline points="20 6 9 17 4 12"></polyline>
      </svg> 
    </button>
  </div>
</template>