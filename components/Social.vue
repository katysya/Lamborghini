<script setup lang="ts">
</script>

<template>
    <ul class="social">
        <li class="social__item">
            <a class="social__link" href="#" target="_blank">
                <img src="../assets/img/social/linkedin.svg" alt="LinkedIn">
            </a>
        </li>
        <li class="social__item">
            <a class="social__link " href="#" target="_blank">
                <img src="../assets/img/social/insta.svg" alt="LinkedIn">
            </a>
        </li>
        <li class="social__item">
            <a class="social__link " href="#" target="_blank">
                <img src="../assets/img/social/facebook.svg" alt="LinkedIn">
            </a>
        </li>
        <li class="social__item">
            <a class="social__link " href="#" target="_blank">
                <img src="../assets/img/social/youtube.svg" alt="LinkedIn">
            </a>
        </li>
    </ul>
</template>

<style lang="scss" scoped>
.social {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 30px;

    &__item {
        width: 40px;
        height: 40px;
        padding: 5px;
        border-radius: 50%;
        background-color: var(--whiteDark);
    }

    &__link {
        display: flex;
        flex-direction: row;
        align-items: center;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    }
}
</style>