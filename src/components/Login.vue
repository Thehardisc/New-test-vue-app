<template>
<div>
    <i class="fa-solid fa-right-to-bracket"></i>
</div>
</template>

<script>
import LoginForm from "./LoginForm.vue";

export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Login",
    components: {
        LoginForm
    }
}
</script>

<style scoped>
i {
    @apply py-3 cursor-pointer w-full text-center;
}
</style>