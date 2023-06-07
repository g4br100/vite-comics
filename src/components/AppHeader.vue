<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "Characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "Tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "Games",
                    url: "#",
                    current: false,
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "News",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="logo">
            <a href="/" class="brand">
                <img src="../assets/img/dc-logo.png" alt="dc">
            </a>
        </div>
        <nav>
            <ul>
                <li v-for="link in links">
                    <a :href="link.url" :class="{ active: link.current }">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header {
    @include center ();
    padding: 1% 5%;

    .logo {
        width: 50%;
        height: 100%;
        @include center ();

        img {
            width: 60px;

        }
    }

    nav {
        width: 50%;

        ul {
            margin: 0;
            @include center ();

            li {
                width: 100%;
                text-align: center;
                margin-right: 10px;
                height: 60px;
                margin-top: 26px;




                a {
                    color: black;
                    display: inline-block;
                    text-transform: uppercase;
                    text-decoration: none;
                    font-weight: 600;
                    font-size: 12px;
                    transition: background 0.3s;
                }

                &:active,
                &:hover {
                    color: $primary-color;
                    border-bottom: 5px solid $primary-color;
                }


            }
        }
    }
}
</style>