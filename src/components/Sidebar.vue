<script setup>
    import urlData from '../assets/data/urls.json'
    import { ref } from 'vue';
    const urls = ref(urlData.sideBar)

</script>

<template>
    <div class="px-3 py-1">
        <a v-for="url in urls.main" :key="url.title"
            class="d-flex justify-content-start btn btn-dark w-100 rounded-4 align-items-center text-center py-2">
            <i :class="url.icon + ' px-2 me-2'"></i>
            {{ url.title }}
        </a>
        <hr>
        <a class="d-flex justify-content-start btn btn-dark w-100 rounded-4 align-items-center text-center py-2">
            You
            <i class="px-2 me-2 bi bi-arrow-right-short"></i>
        </a>
        <a v-for="url in urls.you_section" :key="url.title"
            class="d-flex justify-content-start btn btn-dark w-100 rounded-4 align-items-center text-center py-2">
            <i :class="url.icon + ' px-2 me-2'"></i>
            {{ url.title }}
        </a>
        <hr>
        
    </div>
</template>