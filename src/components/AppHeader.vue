<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    title: "CHARACTERS",
                    href: "/characters",
                    active: false,
                },
                {
                    title: "COMICS",
                    href: "/comics",
                    active: true,
                },
                {
                    title: "MOVIES",
                    href: "/movies",
                    active: false,
                },
                {
                    title: "TV",
                    href: "/tv",
                    active: false,
                },
                {
                    title: "GAMES",
                    href: "/games",
                    active: false,
                },
                {
                    title: "COLLECTIBLES",
                    href: "/collectibles",
                    active: false,
                },
                {
                    title: "VIDEOS",
                    href: "/videos",
                    active: false,
                },
                {
                    title: "FANS",
                    href: "/fans",
                    active: false,
                },
                {
                    title: "NEWS",
                    href: "/news",
                    active: false,
                },
                {
                    title: "SHOP",
                    href: "/shop",
                    active: false,
                }
            ]
        }
    }
}
</script>


<template>

    <div class="container-header">

        <div class="header-left">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>


        <div class="header-right">
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a href="" :class="[link.active === false ? 'n-active' : 'active']"> {{ link.title }}
                    </a>
                </li>
            </ul>
        </div>

    </div>

</template>


<style lang="scss" scoped>
@use "../styles/general.scss" as *;

.container-header {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;

    max-width: 1200px;

    padding: 1rem;
    width: 90%;
    margin: auto;

    .header-left {
        width: 20%;
        text-align: left;

        img {
            padding: .2rem;
            width: 35%;
            max-width: 100px;
        }
    }

    .header-right {
        width: 78%;
        display: flex;
        flex-wrap: wrap;
        justify-content: flex-end;

        ul {
            display: flex;
            flex-wrap: wrap;
            align-items: flex-end;
            gap: .8rem;
        }

        li {
            text-decoration: none;
            list-style-type: none;
            font-size: .8rem;

            a {
                text-decoration: none;
                padding-bottom: 3.6rem;
            }
        }
    }

    .active {
        color: #0082f9;
    }

    .n-active {
        color: black;
    }
}
</style>