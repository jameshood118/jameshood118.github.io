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
            <router-link :to="{path: '/home'}" class="navbar-item">
                Home
            </router-link>
            <router-link :to="{path: '/about'}" class="navbar-item">
                About
            </router-link>
            <router-link :to="{path: '/resume'}" class="navbar-item">
                Resume
            </router-link>
            <router-link :to="{path: '/contact'}" class="navbar-item">
                Contact
            </router-link>
            <router-link :to="{path: '/thoughts'}" class="navbar-item">
                Thoughts
            </router-link>
            <router-link :to="{path: '/profiles'}" class="navbar-item">
                Profiles
            </router-link>
            <router-link :to="{path: '/code'}" class="navbar-item">
                Code Samples
            </router-link>
            <router-link :to="{path: '/sites'}" class="navbar-item">
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
.navbar-item {
  color: white;
}
</style>