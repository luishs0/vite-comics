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
                <li v-for="(link, index) in links"><a href=""> {{ link.title }} </a></li>
            </ul>
        </div>

    </div>

</template>


<style lang="scss" scoped>
.container-header {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;

    max-width: 1200px;



    width: 80%;
    margin: auto;

    .header-left {
        width: 20%;
        text-align: center;

        img {
            padding: .2rem;
            height: 5rem;
        }
    }

    .header-right {
        width: 75%;

        ul {
            display: flex;
            flex-wrap: wrap;
            gap: .8rem;
        }

        li {
            text-decoration: none;
            list-style-type: none;
            font-size: .8rem;

            a {
                text-decoration: none;
                color: black;
            }
        }
    }
}
</style>