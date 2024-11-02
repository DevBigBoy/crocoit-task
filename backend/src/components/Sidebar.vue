<template>
    <div class="min-w-[160px] w-[250px]  transition-all bg-indigo-700 text-white py-10 px-2 ">
        <router-link :to="{name: 'app.dashboard'}"
                     class="flex items-center p-2 mb-1.5 rounded transition-colors hover:bg-black/30">
            <span class="mr-2 text-gray-300">
                <HomeIcon class="w-5"/>
            </span>

            <span class="text-xs">Dashboard</span>
        </router-link>

        <router-link :to="{name: 'app.dashboard'}"
                     class="flex items-center p-2 rounded transition-colors hover:bg-black/30">
            <span class="mr-2 text-gray-300">
                <SwatchIcon class="w-5"/>
            </span>
            <span class="text-xs">Categories</span>
        </router-link>

        <router-link :to="{name: 'app.products'}"
                     class="flex items-center p-2 rounded transition-colors hover:bg-black/30">
            <span class="mr-2 text-gray-300">
                <BuildingStorefrontIcon class="w-5"/>
            </span>
            <span class="text-xs">Products</span>
        </router-link>

        <router-link :to="{name: 'app.dashboard'}"
                     class="flex items-center p-2 rounded transition-colors hover:bg-black/30">
            <span class="mr-2 text-gray-300">
                <TruckIcon class="w-5"/>
            </span>

            <span class="text-xs">Orders</span>
        </router-link>

        <router-link :to="{name: 'app.dashboard'}"
                     class="flex items-center p-2 rounded transition-colors hover:bg-black/30">
            <span class="mr-2 text-gray-300">
                <UsersIcon class="w-5"/>
            </span>
            <span class="text-xs">Users</span>
        </router-link>

        <router-link :to="{name: 'app.dashboard'}"
                     class="flex items-center p-2 rounded transition-colors hover:bg-black/30">
            <span class="mr-2 text-gray-300">
                <UserGroupIcon class="w-5"/>
            </span>
            <span class="text-xs">Customers</span>
        </router-link>

        <router-link :to="{name: 'app.dashboard'}"
                     class="flex items-center p-2 rounded transition-colors hover:bg-black/30">
            <span class="mr-2 text-gray-300">
                <ChartBarIcon class="w-5"/>
            </span>
            <span class="text-xs">Reports</span>
        </router-link>
    </div>
</template>

<script setup>
import { HomeIcon, UserGroupIcon, UsersIcon, SwatchIcon, ChartBarIcon, BuildingStorefrontIcon, TruckIcon } from '@heroicons/vue/24/outline';
</script>

<style scoped>
/* Styles here */
</style>
