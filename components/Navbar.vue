<template>
    <div class="navbar">
        <a class="title">nyanbleh</a>
        <a href="https://github.com/Mewski">
            <nuxt-img src="/a.png"/>
        </a>
    </div>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style scoped>
    .navbar {
        background-color: #0E0F19;
        height: 40px;
        width: 100%;
        position: absolute;
    }
    .title {
        color: #ffffff;
        font-size: 14px;
        margin-top: 12px;
        margin-left: 12px;
        position: absolute;
    }
</style>