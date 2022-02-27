<template> 
<section class="bg-img relative pb-80">
<nav class=" bg-white border-gray-200  sm:px-4 py-2.5  dark:bg-gray-800  justify-around ">

<div class="container flex flex-wrap justify-between items-center mx-auto">
<a href="#" class="flex">
<span class="self-center text-lg text-orange-400 font-semibold whitespace-nowrap dark:text-white">logo</span>
</a>
<div class="flex items-center md:order-2">
<button type="button" class="flex mr-3 text-sm bg-gray-800 rounded-full md:mr-0 focus:ring-4 focus:ring-gray-300 dark:focus:ring-gray-600" id="user-menu-button" aria-expanded="false" data-dropdown-toggle="dropdown">
<span class="sr-only">Open user menu</span>
<i class="fas fa-shopping-bag text-orange-400 text-lg "></i>
</button>

<div class="hidden z-50 my-4 text-base list-none bg-white rounded divide-y divide-gray-100 shadow dark:bg-gray-700 dark:divide-gray-600" id="dropdown">
<div class="py-3 px-4">
<span class="block text-sm text-gray-900 dark:text-white">Bonnie Green</span>
<span class="block text-sm font-medium text-gray-500 truncate dark:text-gray-400">name@flowbite.com</span>
</div>
<ul class="py-1" aria-labelledby="dropdown">
<li>
<a href="#" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Dashboard</a>
</li>
<li>
<a href="#" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Settings</a>
</li>
<li>
<a href="#" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Earnings</a>
</li>
<li>
<a href="#" class="block py-2 px-4 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-200 dark:hover:text-white">Sign out</a>
</li>
</ul>
</div>
<button @click="toggle" data-collapse-toggle="mobile-menu-2" type="button" class="inline-flex items-center p-2 ml-1 text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="mobile-menu-2" aria-expanded="false">
<span class="sr-only">Open main menu</span>
<svg v-if="!isOpen" class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
<svg v-if="isOpen" class=" w-6 h-6" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>
</button>
</div>
<div  :class="isOpen ? 'block':'hidden'" class=" justify-between items-center w-full md:flex md:w-auto md:order-1" id="mobile-menu-2">
<ul class="flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium">
<li>
<a href="#" class="block text-lg py-2 pr-4 pl-3 text-white border-b  border-white    md:p-0 md:pb-2 " aria-current="page">Home</a>
</li>
<li>
<a href="#" class="block text-lg py-2 pr-4 pl-3 text-white   md:p-0 hover:border-b  border-white     md:pb-2    ">Special Menu</a>
</li>
<li>
<a href="#" class="block text-lg py-2 pr-4 pl-3 text-white   md:p-0 hover:border-b  border-white     md:pb-2 ">Foods</a>
</li>
<li>
<a href="#" class="block text-lg  py-2 pr-4 pl-3 text-white   md:p-0 hover:border-b  border-white     md:pb-2 ">Contact Us</a>
</li>
</ul>
</div>
</div>
</nav>
<div class="text-center pt-52  text-white">
    <div class="uppercase text-7xl ">welcome</div>
    <div class="capitalize text-2xl mt-4">fast food & good mood</div>
    <button class="mt-16 bg-orange-400 py-3 px-20 rounded font-bold">All menu</button>
</div>
</section>       

</template>

<script>
export default {
    data(){
        return {
            isOpen:false,
        }
    },
    methods:{
        toggle: function(){
            this.isOpen = !this.isOpen
        }
    }
}
</script>

<style scoped>
nav{
  width: 100%;  
  background-color: transparent;
}
.bg-img {
    background-image: url(../../assets/nathan-dumlao-D4GjwNpXtV0-unsplash.jpg);
    width: 100%;
    background-size: 100% 120%;
}
</style>