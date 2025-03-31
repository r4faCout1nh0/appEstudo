<template>
    <div class="login-container">
        <div class="login-box">
            <svg class="passLogo" xmlns="http://www.w3.org/2000/svg" viewBox="0 -960 960 960">
                <path d="M420-360h120l-23-129q20-10 31.5-29t11.5-42q0-33-23.5-56.5T480-640q-33 0-56.5 23.5T400-560q0 23 11.5 42t31.5 29l-23 129Zm60 280q-139-35-229.5-159.5T160-516v-244l320-120 320 120v244q0 152-90.5 276.5T480-80Zm0-84q104-33 172-132t68-220v-189l-240-90-240 90v189q0 121 68 220t172 132Zm0-316Z"/>
            </svg>
            <form action="submit">
                <input type="email" name="email" id="email" placeholder="Email">
                <input type="password" name="password" id="password" placeholder="Senha">
                <button @click="ExecLogin" >Entrar</button>
            </form>
        </div>
    </div>
</template>

<script setup>
    definePageMeta({
        layout: 'login-page'
    })

    function ExecLogin(e) {
        e.preventDefault();
        console.log('Entrou');
        navigateTo('/home');
    }
</script>

<style lang="scss" scoped>

</style>