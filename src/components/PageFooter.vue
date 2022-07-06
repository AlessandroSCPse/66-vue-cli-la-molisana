<template>
    <footer>
        <div class="container">
            <div class="footer-cols">
                <div class="logo-col">
                    <img src="../assets/img/la-molisana-logo.png" alt="Molisana logo">
                </div>

                <div class="menu-col">
                    <h3>Prodotti</h3>

                    <ul class="footer-menu">
                        <li>
                            <a href="#">Link element</a>
                        </li>

                        <li>
                            <a href="#">Link element</a>
                        </li>

                        <li>
                            <a href="#">Link element</a>
                        </li>

                        <li>
                            <a href="#">Link element</a>
                        </li>
                    </ul>
                </div>

                <div class="menu-col">
                    <h3>Prodotti</h3>

                    <ul class="footer-menu">
                        <li>
                            <a href="#">Link element</a>
                        </li>

                        <li>
                            <a href="#">Link element</a>
                        </li>

                        <li>
                            <a href="#">Link element</a>
                        </li>

                        <li>
                            <a href="#">Link element</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "PageFooter"
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

footer {
    padding-top: 30px;

    .footer-cols {
        display: flex;
        justify-content: space-between;
    }

    .menu-col {
        h3 {
            color: $brand_main_color;
            font-size: 25px;
        }
    }

    .footer-menu {
        margin-top: 15px;

        li {
            padding: 2px 0;

            a {
                color: black;
                text-decoration: none;
                font-size: 22px;
            }
        }
    }
}
</style>