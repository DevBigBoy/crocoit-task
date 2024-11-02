<template>
    <div class="min-h-full bg-gray-200 flex">
        <!--==================== Sidebar ===============-->
        <Sidebar :class="{'-ml-[250px]': !sidebarOpened}"/>
        <!--==================== Sidebar ==============-->

        <div class="flex-1">
            <!--==================== Navbar ==============-->
            <Navbar @toggle-sidebar="toggleSidebar"></Navbar>
            <!--==================== Navbar ==============-->

            <main class="p-6">
                <router-view></router-view>
            </main>
        </div>

    </div>
</template>

<script setup>
import {ref, onMounted, onUnmounted} from 'vue';
import Sidebar from "./Sidebar.vue";
import Navbar from "./Navbar.vue";

const sidebarOpened = ref(true);

function toggleSidebar() {
    sidebarOpened.value = !sidebarOpened.value
}

function updateSidebarState() {
    sidebarOpened.value = window.outerWidth > 768;
}

onMounted(() => {
    updateSidebarState();
    window.addEventListener('resize', updateSidebarState)
})

onUnmounted(() => {
    window.removeEventListener('resize', updateSidebarState)
})

</script>

<style scoped>

</style>
