<!-- <template>
    <form class="login-form">
    <div class="container">
    <div class="us-name">
    <label>Username</label>
    <input name="user" placeholder="Username" type="text" class="input-log text-black"/>
    </div>
    <div class="pass-us">
    <label>Password</label>
    <input name="pass" placeholder="Password" type="password" class="input-log text-black">
    </div>
    <div class="remember-me" >
    <label>Remember Me</label>
    <input type="checkbox" name="rememberme">
    </div>
    <div>
    <input type="submit" value="Login" class="input-btn">
    </div>
    </div>
    </form>
</template>
<script>
export default {
    name: 'LoginForm'
}
</script>
<style scoped>
.login-form {
    @apply flex justify-center text-gray-100;
}
.container {
    @apply flex flex-col w-1/5 p-4 bg-primary mt-3 border-black border-2 ;
}
.pass-us {
    @apply flex flex-col my-2 items-center pb-3 border-b-[1px] border-b-gray-600;
}
.us-name {
    @apply flex flex-col my-1 items-center;
}
.remember-me {
    @apply flex flex-col items-center;
}
.remember-me input {
    @apply mt-[2px]
}
.input-log {
    @apply w-10/12 
}
.input-btn {
    @apply bg-black mt-2 px-2 py-1 text-[16px] font-bold w-10/12 
}
</style> -->

<template>
    <div>
    <form class="modal-contentanimate" >
        <div class="display-form" :class="[toggleIfPressed ? 'block' : 'hidden' ]">
        <label>Login Page</label>
        <p>{{ toggleIfPressed }}</p>
        </div>
    </form>
    </div>
</template>

<script>
export default {
    name: 'LoginForm',
    props: {
        toggleIfPressed: Boolean,
    },
}
</script>

<style scoped>
.modal-contentanimate {
    @apply block
}
</style>