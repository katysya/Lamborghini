<script setup lang="ts">
</script>

<template>
    <footer class="footer">
        <div class="container">
            <NuxtLink to="/" class="footer__logo">
                <img src="../assets/img/footer/logo.svg" alt="Logo">
            </NuxtLink>
            <div class="footer__info">
                <a class="footer__link" href="#">Legal notice</a>
                <a class="footer__link" href="#">Privacy Policy</a>
                <a class="footer__link" href="#">Cookie Policy</a>
                <a class="footer__link" href="tel: +74951864746">+ 7 (495) 186 47 46</a>
            </div>
            <p class="footer__desc">
                *Please note that this website is for informational purposes only and under no circumstances is a public
                offer, determined by the provisions of Art. 437 Civil Code of the Russian Federation. For detailed
                information about the availability and cost of these goods and (or) services, about terms and conditions of
                the promotions, please contact sales managers. You can find the address and phone number in section
                Contacts.
            </p>
            <div class="footer__bottom">
                <p class="footer__copy">© 2000-2023 lamborghini</p>
                <Social />
                <Language />
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
.footer {
    color: var(--white);
    padding: 16px 0 60px 0;

    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    &__info {
        width: 100%;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        padding-bottom: 40px;
        gap: 70px;
        margin-top: 50px;
        border-bottom: 1px solid var(--whiteDark);

        a {
            font-weight: 400;
            font-size: 16px;
        }
    }

    &__logo {
        img {
            width: 75px;
            height: 78px;
        }
    }

    &__desc {
        margin-top: 32px;
        font-size: 16px;
        text-align: center;
        line-height: 23px;
        max-width: 846px;
    }

    &__bottom {
        margin-top: 36px;
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 80px;
    }
}
</style>