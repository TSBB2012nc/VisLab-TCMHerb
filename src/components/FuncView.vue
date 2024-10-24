<script setup>
import FigView from './funcviews/FigView.vue';
import MapView from './funcviews/MapView.vue';
import TextView from './funcviews/TextView.vue';

</script>

<template>
    <div class="func-view flex-row content-center w-3/4 h-[100vh] border-4 border-dashed">
        <TextView />
        <FigView />
        <MapView />
    </div>
</template>