<template>
    <header class="fixed bg-white w-full py-[10px] top-0">
       <div class="container max-w-[1440px] mx-auto  rounded-full shadow-md p-[10px_30px] h-[70px] w-full border border-[#ccc] flex items-center justify-between">
            <NuxtImg src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS5VcuqH0iTYvV2x9ioVtJx2DkidXedViZtqw&s" class="w-[150px] h-[40px]"/>

            <ul class="flex items-center gap-[20px]">
                <li 
                v-for="(route, index) in routes"
                :key="index"
                class="cursor-pointer hover:underline duration-300 hover:text-green-600 font-medium">
                    <NuxtLink :to="route.path">{{route.name}}</NuxtLink>
                </li>
                
            </ul>
       </div>
    </header>
</template>

<script setup>
const routes = [
  { name: 'Home', path: '/' },
  { name: 'Products', path: '/products' },
  { name: 'Pricing', path: '/pricing' },
  { name: 'Sign in', path: '/sign-in' }
]
</script>


<style scoped>

</style>