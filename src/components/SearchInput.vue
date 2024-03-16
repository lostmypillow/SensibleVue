<script setup>
const title = defineModel()

</script>

<template>
    <div class="flex flex-row gap-2">
        <input id="SearchInput" class="border-2 p-4 bg-zinc-100 rounded-full h-14 focus:shadow-2xl" type="text" v-model="title"
            placeholder="Search for movies" />
        <button @click="$emit('searchMovies')" id="SearchButton" class="border-2 rounded-full h-14 w-14 p-2 flex items-center justify-center bg-black">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                class="feather feather-search">
                <circle cx="11" cy="11" r="8"></circle>
                <line x1="21" y1="21" x2="16.65" y2="16.65"></line>
            </svg>

        </button>
    </div>
</template>
