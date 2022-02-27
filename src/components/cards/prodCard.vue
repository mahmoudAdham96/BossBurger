<template>
    <div class="container mx-auto mt-10">
        <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-20  justify-center">
            <card class=" bg-white  border-gray-100 rounded-lg  hover:shadow-lg align-center" v-for="prod in 20" :key="prod">
                
                <a href="">
                <img src="../../assets/3.png" class="rounded-xl" />
                </a>
                <p class="px-2 font-semibold pt-3 pb-2 capitalize flex justify-between"> <span>beef burger</span> <span class="text-orange-400">35.00 Rs</span> </p>                
                <p class="px-2 py-2 mb-5 text-gray-500">
                    it is a long established fact that a reader will be distracted is a long established fact that a reader will be distracted
                </p>
                <button class="bg-orange-300 hover:bg-orange-200 w-full py-2 text-white rounded-lg">Add to cart</button>
                
            </card>
        </div>
    </div>
</template>