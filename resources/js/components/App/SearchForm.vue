<template>
    <form class="w-[600px] h-[80px] flex items-center" action="">
        <TextInput type="text" 
                    class="block w-full" 
                    v-model="form.search" 
                    autocomplete 
                    placeholder="Search For Cloths"/>
    </form>
</template>

<script setup>
import TextInput from "@/components/TextInput.vue";
import {useForm} from "@inertiajs/vue3";

const form = useForm({
    search: ''
})
</script>