<template>
    <header>
        <!-- Header logo -->
        <div class="logo">
            <img src="../assets/img/la-molisana-logo.png" alt="Molisana logo">
        </div>

        <!-- Header nav -->
        <nav>
            <ul class="menu">
                <li v-for="link, index in menuLinks" :key="index" :class="{ 'current': link.current }">
                    <a :href="link.url">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: "PageHeader",
    data() {
        return {
            menuLinks: [
                {
                    text: 'Home',
                    url: '#',
                    current: false
                },
                {
                    text: 'Prodotti',
                    url: '#',
                    current: true
                },
                {
                    text: 'Chi siamo',
                    url: '#',
                    current: false
                },
                {
                    text: 'Contatti',
                    url: '#',
                    current: false
                }
            ],
        };
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

header {
    // Logo
    .logo {
        text-align: center;

        img {
            width: 300px;
            display: inline-block;
        }
    }

    // Nav
    .menu {
        margin: 30px 0;
        display: flex;
        justify-content: center;

        li {
            padding: 10px;

            a {
                color: black;
                text-decoration: none;
                font-size: 25px;
            }

            &.current {
                background-color: $brand_secondary_color;   
            }
        }
    }
}


</style>