<template>
    <nav class="min-w-[200px]">
        <div class="h-[80px] px-3 flex items-center gap-3">
            <Link :href="route('dashboard')">
            <ApplicationLogo class="block h-9 w-auto fill-current text-gray-800" />
            </Link>
            WDM'System
        </div>
        <div class="px-3">
            <CreateNewDropdown />

            <div class="py-3">
                <NavLink href="/">Add Items</NavLink>
                <NavLink href="/">Edit Items</NavLink>
                <NavLink href="/">Update Items</NavLink>
                <NavLink href="/">Delete Items</NavLink>
            </div>
        </div>
    </nav>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';
import ApplicationLogo from "@/components/ApplicationLogo.vue";
import CreateNewDropdown from "@/components/app/CreateNewDropdown.vue";
import NavLink from "@/components/NavLink.vue";
</script>