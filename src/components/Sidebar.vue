<script setup>
import { ref } from 'vue';

const isCollapsed = ref(true);

const toggleSidebar = () => {
  isCollapsed.value = !isCollapsed.value;
};
</script>
<template>
	<div class="sidebar flex flex-col h-[100vh] p-3 dark:bg-gray-50 dark:text-gray-800 duration-700 ease-in-out" :class="isCollapsed ? 'w-16' : 'w-60'" >
		<div class="space-y-3">
			<div class="flex items-center justify-between">
				<h2 :class="isCollapsed ? 'hidden': ''">Vis Herb</h2>
				<button class="p-2" @click="toggleSidebar">
					<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512" class="w-5 h-5 fill-current dark:text-gray-800">
						<rect width="352" height="32" x="80" y="96"></rect>
						<rect width="352" height="32" x="80" y="240"></rect>
						<rect width="352" height="32" x="80" y="384"></rect>
					</svg>
				</button>
			</div>
			<div class="relative" :class="isCollapsed ? 'hidden': ''">
				<span class="absolute inset-y-0 left-0 flex items-center py-4">
					<button type="submit" class="p-2 focus:outline-none focus:ring">
						<svg fill="currentColor" viewBox="0 0 512 512" class="w-5 h-5 dark:text-gray-600">
							<path d="M479.6,399.716l-81.084-81.084-62.368-25.767A175.014,175.014,0,0,0,368,192c0-97.047-78.953-176-176-176S16,94.953,16,192,94.953,368,192,368a175.034,175.034,0,0,0,101.619-32.377l25.7,62.2L400.4,478.911a56,56,0,1,0,79.2-79.195ZM48,192c0-79.4,64.6-144,144-144s144,64.6,144,144S271.4,336,192,336,48,271.4,48,192ZM456.971,456.284a24.028,24.028,0,0,1-33.942,0l-76.572-76.572-23.894-57.835L380.4,345.771l76.573,76.572A24.028,24.028,0,0,1,456.971,456.284Z"></path>
						</svg>
					</button>
				</span>
				<input type="search" name="Search" placeholder="搜索本草" class="w-full py-2 pl-10 text-sm dark:border- rounded-md focus:outline-none dark:bg-gray-100 dark:text-gray-800 focus:dark:bg-gray-50">
			</div>
		</div>

	</div>
</template>