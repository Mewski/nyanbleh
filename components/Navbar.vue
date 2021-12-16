<template>
  <div class="navbar">
    <a class="title" href="/">nyanbleh</a>
    <div class="socials">
      <a href="https://discord.gg/bark">
        <img class="navbar-icon" src="/Discord-Bubble-Light-64px.png" />
      </a>
      <a href="https://github.com/Mewski">
        <img class="navbar-icon" src="/GitHub-Mark-Light-64px.png" />
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style scoped>
.navbar {
  background-color: #0e0f19;
  height: 40px;
  width: 100%;
  position: absolute;
}
.title {
  color: #dcdcdc;
  font-size: 14px;
  margin-top: 12px;
  margin-left: 12px;
  position: absolute;
  text-decoration: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.title:hover {
  color: #857caf;
}
.socials {
  right: 5px;
  position: absolute;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.navbar-icon {
  margin-right: 10px;
  margin-top: 8px;
  width: 24px;
  height: 24px;
}
</style>
