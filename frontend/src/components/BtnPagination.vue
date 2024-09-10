<template>
    <button :type="buttonType" :disabled="disabled" @click="$emit('handleClick')"
    class="flex justify-center align-center bg-sky-500 p-2 px-3 rounded-xl font-bold text-gray-200 hover:bg-sky-800 disabled:bg-gray-500">{{ buttonName }}
    </button>
</template>

<script setup>
defineProps(["buttonName", "buttonType", "disabled"])
defineEmits(["handleClick"])
</script>