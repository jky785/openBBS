<template>
    <div>
        <nav>
            <Nuxt-link to="/"><h1>LOGO</h1></Nuxt-link>
            <UButton to="/channal_list" color="primary" variant="ghost" label="채널 목록" />
            <UTextarea v-model="value" :rows="1"  placeholder="Search..." />
            <UButton to="/member/login" icon="i-heroicons-user" size="sm" color="primary" square variant="ghost" />
        </nav>
        <nuxt />
    </div>
</template>
<script>

</script>