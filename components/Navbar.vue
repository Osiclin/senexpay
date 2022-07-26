<template>
  <div class="container">
    <Logo/>
    <div class="menuWrapper">
        <nav class="menu">
            <nuxt-link class="link" v-for="(item, index) in menu" :key="index" :to="item">{{ item }}</nuxt-link>
        </nav>
        <div class="right">
            <nuxt-link class="link" to="/login">Log in</nuxt-link>
            <Button bgcolor="#1265FB" color="#ffffff" radius="4px">Get Started</Button>
            <IconNigeriaFlag/>
            <IconFlagDropdown/>
        </div>
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
    padding: 1rem 2rem;
    width: 100%;
    margin: 0 auto;
    position: fixed;
    z-index: 4;
}
.link{
    font-size: 1.2rem;
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
.menuWrapper{
    display: flex;
    align-items: center;
}
.menu{
    margin-right: 6rem;
}
@media screen and (max-width: 1000px) {
    .menu{
        display: none;
    }
}
</style>