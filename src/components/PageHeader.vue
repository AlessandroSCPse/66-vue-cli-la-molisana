<template>
    <header>
        <!-- Header logo -->
        <div class="logo">
            <img src="../assets/img/la-molisana-logo.png" alt="Molisana logo">
        </div>

        <!-- Header nav -->
        <nav>
            <ul class="menu">
                <li>
                    <a href="#">Home</a>
                </li>

                <li class="current">
                    <a href="#">Prodotti</a>
                </li>

                <li>
                    <a href="#">Chi siamo</a>
                </li>

                <li>
                    <a href="#">Contatti</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: "PageHeader"
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