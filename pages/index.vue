<template>
    <div>
        <NuxtLink to="/login">Login</NuxtLink>
    </div>
</template>

<script setup>
    definePageMeta({
        layout: false
    })

    import { useRouter } from 'vue-router'
    import { onMounted } from 'vue'

    const router = useRouter()

    onMounted(() => {
        router.push('/login')
    })

</script>

<style lang="scss" scoped>

</style>