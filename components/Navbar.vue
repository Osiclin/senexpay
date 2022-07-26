<template>
  <div class="container">
    <Logo/>
    <nav class="menu">
        <nuxt-link class="link" v-for="(item, index) in menu" :key="index" :to="item">{{ item }}</nuxt-link>
    </nav>
    <div class="right">
        <next-link class="link" to="/login">Log in</next-link>
        <Button bgcolor="#1265FB" color="#ffffff" radius="4px">Get Started</Button>
        <IconNigeriaFlag/>
        <IconFlagDropdown/>
    </div>
  </div>
</template>

<script>
import Logo from './Logo.vue';
import { menu } from '../mocks/menu';
import Button from './Button.vue';
import IconNigeriaFlag from './icons/IconNigeriaFlag.vue';
import IconFlagDropdown from './icons/IconFlagDropdown.vue';

export default {
    name: "NuxtNavbar",
    components: { Logo, Button, IconNigeriaFlag, IconFlagDropdown },
    data() {
        return {
            menu
        }
    }
}
</script>

<style scoped>
.container{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1rem;
    max-width: 1400px;
    margin: 0 auto;
}
.link{
    font-size: 1.5rem;
    margin-right: 2rem;
    text-decoration: none;
    letter-spacing: 0px;
    color: #FFFFFF;
    opacity: 1;
}
.right{
    display: flex;
    align-items: center;
}
@media screen and (max-width: 1000px) {
    .menu{
        display: none;
    }
}
</style>