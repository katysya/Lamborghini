<script setup lang="ts">

import Language from '../components/Language.vue';

</script>

<template>
    <header class="header">
        <div class="container">
            <div></div>
            <nav class="header__nav">
                <ul class="header__menu">
                    <li class="header__link">
                        <NuxtLink to="/">Models</NuxtLink>
                    </li>
                    <li class="header__link">
                        <NuxtLink to="/">Service</NuxtLink>
                    </li>
                    <li class="header__link">
                        <NuxtLink to="/">About us</NuxtLink>
                    </li>
                    <li class="header__link">
                        <NuxtLink class="header__logo" to="/">
                            <img src="../assets/img/header/logo.svg" alt="Logo">Lamborgini
                        </NuxtLink>
                    </li>
                    <li class="header__link">
                        <NuxtLink to="/">Events</NuxtLink>
                    </li>
                    <li class="header__link">
                        <NuxtLink to="/">Features</NuxtLink>
                    </li>
                    <li class="header__link">
                        <NuxtLink to="/">Contact us</NuxtLink>
                    </li>
                </ul>
            </nav>
            <Language />
        </div>
    </header>
</template>

<style lang="scss" scoped>
.header {
    padding-top: 7px;
    .container {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        color: var(--whiteDark);
    }

    &__menu {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 50px;
    }

    &__logo {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 8px;
        text-transform: uppercase;
        font-size: 20px;
        font-weight: 500;

        img {
            width: 40px;
            height: 46px;
        }
    }
}
</style>