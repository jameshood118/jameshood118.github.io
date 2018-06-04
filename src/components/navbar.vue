<template>
    <nav class="navbar is-dark" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
            <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false">
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
            </a>
        </div>
        <div class="navbar-menu">
            <div class="navbar-start"></div>
            <router-link :to="{path: '/home'}" class="navbar-item has-text-white">
                Home
            </router-link>
            <router-link :to="{path: '/about'}" class="navbar-item has-text-white">
                About
            </router-link>
            <router-link :to="{path: '/resume'}" class="navbar-item has-text-white">
                Resume
            </router-link>
            <router-link :to="{path: '/contact'}" class="navbar-item has-text-white">
                Contact
            </router-link>
            <router-link :to="{path: '/thoughts'}" class="navbar-item has-text-white">
                Thoughts
            </router-link>
            <router-link :to="{path: '/profiles'}" class="navbar-item has-text-white">
                Profiles
            </router-link>
            <router-link :to="{path: '/code'}" class="navbar-item has-text-white">
                Code Samples
            </router-link>
            <router-link :to="{path: '/sites'}" class="navbar-item has-text-white">
                Sites
            </router-link>
            <div class="navbar-end"></div>
        </div>

    </nav>
</template>

<script>
export default {
    name: "Navbar"

}
</script>

<style scoped>
.navbar-item:hover {
  color: hsl(0, 0%, 96%);
  background-color: hsl(0, 0%, 21%);
}
</style>