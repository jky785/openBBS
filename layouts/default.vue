<template>
    <div>
        <nav class="navbar">
            <div class="logo">
                <Nuxt-link to="/"><h2 style="font-size:30px;">LOGO</h2></Nuxt-link>
            </div>
            <div clss="menu">
                <UButton to="/boards" color="gray" variant="ghost" label="게시판 목록" />
            </div>
            <div class="search">
                <UTextarea :rows="1"  placeholder="Search..." />
                <UButton icon="i-heroicons-magnifying-glass" size="sm" color="gray" square variant="solid" />
            </div>
            <div class="user">
                <UButton to="/member/login" icon="i-heroicons-user" size="sm" color="gray" square variant="ghost" />
            </div>
        </nav>
        <slot />
        <p>openBBS</p>
    </div>
</template>

<script>
</script>

<style>
    .navbar{
        justify-content: space-between;
        background-color: #525252;
        display: flex;
        align-items: center;
        height: 40px;
    }
    .search{
        display: flex;
    }
    .logo{
        box-sizing: content-box;
        padding: 0 12px;
        height: 40px;
        flex: 1 0 auto;
        display: flex;
        align-items: center;
    }
    .user{
        padding: 0 12px;
    }
    .menu{
        padding: 0 12px;
    }
</style>