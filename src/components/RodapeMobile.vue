<script setup>
import CartPlus from 'vue-material-design-icons/CartPlus.vue';
import Account from 'vue-material-design-icons/Account.vue';
import Menu from 'vue-material-design-icons/Menu.vue';
import Home from 'vue-material-design-icons/Home.vue';
import { useScreen } from '@/composables/RodapeMobile';
const { isMobile } = useScreen();

</script>
<template>
<div v-if="isMobile" class="footer-mobile">
    <button><CartPlus/></button>
    <button><Account/></button>
    <button><Home/></button>
    <Menu/>
    </div>
</template>
<style>
.footer-mobile{
width: 100%;
height: 50px;
background-color: #e64a38;
display: flex;
justify-content: center;
align-items: center;
gap: 10%;
position: fixed;
bottom: 0;
}
button {
    background-color: transparent;
    border: transparent;
}
</style>