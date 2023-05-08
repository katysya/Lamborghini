<script setup lang="ts">
</script>

<template>
    <div class="language">
        <button class="language__button language__button--active">RU</button>
        <button class="language__button">EN</button>
    </div>
</template>

<style lang="scss" scoped>
.language {
    display: flex;
    flex-direction: row;
    align-items: center;
    gap: 20px;

    &__button {
        border: 0;
        background-color: transparent;
        color: currentColor;
        transition: color 0.3s, font-weight 0.3s;
        color: var(--whiteDark);

        &--active {
            font-weight: 700;
            color: var(--white);
        }
    }
}
</style>