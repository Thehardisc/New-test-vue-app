<template>
<div>
    <i @click="$emit('toogleLoginTab')" class="fa-solid fa-right-to-bracket"></i>
</div>
</template>

<script>
export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Login",
    components: {
    },
}
</script>

<style scoped>
i {
    @apply py-3 cursor-pointer w-full text-center;
}
</style>