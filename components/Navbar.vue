<template>
  <div class="navbar" :class="{ scrolled: !view.atTopOfPage }">
    <NuxtLink class="title" to="/">nyanbleh</NuxtLink>
    <div class="seperator" />
    <div class="nav">
      <NuxtLink class="nav-link" to="/projects">projects</NuxtLink>
      <NuxtLink class="nav-link" to="/about">about me</NuxtLink>
      <NuxtLink class="nav-link" to="/donate">donate</NuxtLink>
      <NuxtLink class="nav-link" to="/dashboard">dashboard</NuxtLink>
    </div>
    <div class="socials">
      <a href="https://discord.gg/bark">
        <img class="navbar-icon" src="/img/Discord-Bubble-Light-64px.png" />
      </a>
      <a href="https://github.com/Mewski">
        <img class="navbar-icon" src="/img/GitHub-Mark-Light-64px.png" />
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
  data() {
    return {
      view: {
        atTopOfPage: true,
      },
    }
  },
  beforeMount() {
    window.addEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll() {
      if (window.pageYOffset > 0) {
        if (this.view.atTopOfPage) this.view.atTopOfPage = false
      } else {
        if (!this.view.atTopOfPage) this.view.atTopOfPage = true
      }
    },
  },
}
</script>

<style scoped>
.navbar {
  background-color: #0e0f19;
  height: 40px;
  width: 100%;
  position: fixed;
  z-index: 99999;
}
.navbar.scrolled {
  box-shadow: 0 4px 4px rgba(0, 0, 0, 0.2);
}
.title {
  color: #dcdcdc;
  font-size: 14px;
  margin-top: 12px;
  margin-left: 12px;
  position: absolute;
  text-decoration: none;
  user-select: none;
}
.nav-link {
  color: #dcdcdc;
  font-size: 14px;
  top: 8px;
  margin-left: 12px;
  position: relative;
  text-decoration: none;
}
.title:hover {
  color: #857caf;
}
.nav-link:hover {
  color: #857caf;
}
.socials {
  right: 5px;
  position: absolute;
}
.navbar-icon {
  margin-right: 10px;
  margin-top: 8px;
  width: 24px;
  height: 24px;
}
.seperator {
  height: 18px;
  margin-top: 11px;
  width: 1px;
  background-color: #4b4b4b;
  position: absolute;
  left: 85px;
}
.nav {
  position: absolute;
  left: 90px;
  height: 100%;
}
</style>
