<script setup>
defineProps({
    type: {
        type: String,
        default: 'button',
    },
});
</script>

<template>
    <button :type="type" class="text-center px-4 py-2 bg-secondary border border-transparent rounded-full text-xs text-white tracking-widest active:scale-95 disabled:active:scale-100 disabled:cursor-not-allowed disabled:opacity-50 disabled:bg-gray-400 focus:outline-none focus:ring-0 transition ease-in-out duration-100">
        <slot />
    </button>
</template>
