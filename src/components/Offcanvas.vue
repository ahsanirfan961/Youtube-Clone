<script setup>
    import { ref, onMounted } from 'vue';
    import Sidebar from './Sidebar.vue';

</script>

<template>
    <div class="offcanvas offcanvas-start" tabindex="-1" id="offcanvas" aria-labelledby="offcanvasLabel">
        <div class="offcanvas-header py-2">
            <div class="d-flex">
                <button class="btn" data-bs-toggle="offcanvas" type="button" data-bs-target="#offcanvas">
                    <i class="bi bi-list" style="font-size: 1.5rem;"></i>
                </button>
                <a href="/" class="d-flex align-items-center link-body-emphasis text-decoration-none">
                    <img src="../assets/images/logo.png" alt="logo" width="90">
                </a>
            </div>
        </div>
        <div class="offcanvas-body p-0 m-0">
            <Sidebar/>
        </div>
    </div>
</template>

<style>
    .offcanvas {
        width: 250px !important;
    }
</style>