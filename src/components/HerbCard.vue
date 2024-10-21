<script setup>
const herb_info = {
    'chinese_name':'人参',
    'eng_name':'Ginseng',
    'latin_name':'Panax ginseng C. A. Mey.'
}
</script>
<template>
    <div class="herb-card h-[15rem] w-full">
        <div href="#"
            class="flex flex-col items-center bg-white border border-gray-200 rounded-lg shadow md:flex-row hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700">
            <img class="object-cover w-full rounded-t-lg h-96 md:h-[13rem] md:w-48 md:rounded-none md:rounded-s-lg"
                src="https://image.zhongyibaike.com/image/%E4%BA%BA%E5%8F%82/%E4%BA%BA%E5%8F%82.jpg" alt="">
            <div class="flex flex-col justify-between p-4 leading-normal">
                <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">{{ herb_info.chinese_name }}
                </h5>
                <h6>{{ herb_info.eng_name }}</h6>
                <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">Here are the biggest enterprise technology
                    acquisitions of 2021 so far, in reverse chronological order.</p>
            </div>
        </div>
    </div>
</template>